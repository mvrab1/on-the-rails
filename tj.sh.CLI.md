tj.sh — task journal writer + state-machine wrappers

  new                                       interactive: GUID + spec_set
  propose  <goal> <prob> <act> <test>       agent-driven spec_set + zenity accept
           [--task-id <id>] [--doc <path>]    --doc stages a detail .md and
           [--files f1 f2 ...]                commits on accept (T-2fd9c35e);
                                              --files names spec-time files
                                              that begin will auto-claim
  accept   <task_id>                        proposed → accepted (human zenity);
                                              commits detail doc if --doc used
  amend    <task_id> <goal> <prob> <act>    revise spec on a working/accepted
           <test> [--doc <p>] [--files ...]   task; zenity-gated re-acceptance
  begin    <task_id>                        accepted → working (claims session;
                                              auto-claims spec-time files;
                                              [files...] arg removed — use
                                              --files at propose, or claim post)
  submit   <task_id>                        working → testing
  deny     <task_id>                        testing → working
  complete <task_id>                        testing → completed (human zenity)
  abandon  <task_id>                        any → abandoned (human zenity)
  reopen   <task_id>                        completed → working (human zenity)
  park     <task_id>                        session_release; stays working
  resume   <task_id>                        session_claim; stays working
  code     <task_id> <files...> [-m msg]    code_change with HEAD sha
  claim    <task_id> <files...>             extend files_claimed (post-accept)
  release  <task_id> <files...>             remove files from files_claimed
  test     <task_id> <pass|fail> [summary]  test_run
  note     <task_id> <text>                 note (cognitive log; non-mutating)
  append   <event> <task_id> [k=v...]       raw append (escape hatch)
  state    [task_id]                        print fold (json)
  list     [<state>|--mine]                 recency-sorted three-column listing
  spec     <task_id>                        print latest spec
  history  <task_id>                        print all events for task
  whoami   [<session_id>]                   tasks owned (default current sid)
