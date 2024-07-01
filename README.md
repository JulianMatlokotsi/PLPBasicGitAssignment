I created a folder on my local drive and added a text file then did the following

matlo@Julian MINGW64 ~
$ cd c:/

matlo@Julian MINGW64 /c
$ git remote add https://github.com/JulianMatlokotsi/PLPBasicGitAssignment.git
fatal: not a git repository (or any of the parent directories): .git

matlo@Julian MINGW64 /c
$ git init
Initialized empty Git repository in C:/.git/

matlo@Julian MINGW64 /c
$ cd PLPBasicGitAssignment

matlo@Julian MINGW64 /c/PLPBasicGitAssignment
$  git remote add https://github.com/JulianMatlokotsi/PLPBasicGitAssignment.git
fatal: detected dubious ownership in repository at 'C:/'
'C:/' is owned by:
        NT SERVICE/TrustedInstaller (S-1-5-80-956008885-3418522649-1831038044-1853292631-2271478464)
but the current user is:
        JULIAN/matlo (S-1-5-21-2267751533-3450488606-1530636249-1001)
To add an exception for this directory, call:

        git config --global --add safe.directory C:/

matlo@Julian MINGW64 /c/PLPBasicGitAssignment
$ git init
Initialized empty Git repository in C:/PLPBasicGitAssignment/.git/

matlo@Julian MINGW64 /c/PLPBasicGitAssignment (master)
$ ls
hello.txt

matlo@Julian MINGW64 /c/PLPBasicGitAssignment (master)
$ git remote add https://github.com/JulianMatlokotsi/PLPBasicGitAssignment.git
usage: git remote add [<options>] <name> <url>

    -f, --[no-]fetch      fetch the remote branches
    --[no-]tags           import all tags and associated objects when fetching
                          or do not fetch any tag at all (--no-tags)
    -t, --[no-]track <branch>
                          branch(es) to track
    -m, --[no-]master <branch>
                          master branch
    --[no-]mirror[=(push|fetch)]
                          set up remote as a mirror to push to or fetch from


matlo@Julian MINGW64 /c/PLPBasicGitAssignment (master)
$ git remote add origin https://github.com/JulianMatlokotsi/PLPBasicGitAssignment.git

matlo@Julian MINGW64 /c/PLPBasicGitAssignment (master)
$ ls

matlo@Julian MINGW64 /c/PLPBasicGitAssignment (master)
$ ls
hello.txt

matlo@Julian MINGW64 /c/PLPBasicGitAssignment (master)
$ git add hello.txt

matlo@Julian MINGW64 /c/PLPBasicGitAssignment (master)
$ git commit -m "Add hello.txt with a greeting"
[master (root-commit) e960ebf] Add hello.txt with a greeting
 1 file changed, 1 insertion(+)
 create mode 100644 hello.txt

matlo@Julian MINGW64 /c/PLPBasicGitAssignment (master)
$ git push -u origin main
error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/JulianMatlokotsi/PLPBasicGitAssignment.git'

matlo@Julian MINGW64 /c/PLPBasicGitAssignment (master)
$ git push -u origin master
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 244 bytes | 61.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote:
remote: Create a pull request for 'master' on GitHub by visiting:
remote:      https://github.com/JulianMatlokotsi/PLPBasicGitAssignment/pull/new/master
remote:
To https://github.com/JulianMatlokotsi/PLPBasicGitAssignment.git
 * [new branch]      master -> master
branch 'master' set up to track 'origin/master'.

matlo@Julian MINGW64 /c/PLPBasicGitAssignment (master)
