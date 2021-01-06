# school-tools
A collection of tools I built for working with GitHub Classrooms


I need to shorten the names of a lot of these scripts, but basically:

   * `make_new_assingment_repo` is a bash script that lets you create a new GitHub repo with from a template from the command line.  I'm using it to create a new repo from  my template java assignment repo and run a sed search and replace to make it use new classes in the repo itself and in tests, then adding any starter code.

   * `pull_down_student_repos` is used to pull down all current student repos for a given assignment (requires an ssh key and an authorization token be pre-configured) from your private organization using private repos.  This is useful to push out updates to tests and assignments after students have already begun working.
   
   * After rewriting the files, you may get a "fatal: unkown index entry format" error.  To fix `rm -f .git/index` followed by `git reset`.
