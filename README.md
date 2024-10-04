# Ch2.5
# Exercise: Managing Git Remotes

## Step 1
Familiarize yourself with the repository by checking the repository history, file structure, file contents, etc.

## Step 2
Identify the name of the git remote this repository was cloned from using:
```bash
$ git remote
```

## Step 3
The URL of the remote can be obtained using:
```bash
$ git remote -v
```
The output should indicate that the URL of the remote is the same as the URL this repository was cloned from.

## Step 4
To find out more details about the remote, you can type:
```bash
$ git remote show <remoteName>
```
where `<remoteName>` should be substituted with the actual name of the remote obtained at `Step 2`.

## Step 5
Run the following command:
```bash
$ git log --decorate
```
The output should indicate that the current branch `master` points to the same commit as the remote branch `<remoteName>/master` (where `<remoteName>` was identified at `Step 2`)

## Step 6
Run the `./chaos_monkey1.sh` script.

## Step 7
Find out the new name of the remote (which still points to the URL this repository was cloned from).

## Step 8
Run the `./chaos_monkey2.sh` script.

## Step 9
Find out the name of the newly added remote that points to the `URL_OF_SOME_FAKE_GITHUB_REPOSITORY` URL.

## Step 10 (Optional)
You can remove a remote using:
```bash
$ git remote remove <remoteName>
```
