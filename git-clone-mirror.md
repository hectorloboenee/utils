# Git Repository Migration Using Mirror

## 1. Clone the source repository

```bash
git clone --mirror https://github.com/SOURCE_ORGANIZATION/repository.git
```

## 2. Enter the repository

```bash
cd repository.git
```

## 3. Set the destination repository

```bash
git remote set-url origin https://github.com/TARGET_ORGANIZATION/repository.git
```

## 4. Verify the remote

```bash
git remote -v
```

Expected output:

```text
origin  https://github.com/SOURCE_ORGANIZATION/repository.git (fetch)
origin  https://github.com/TARGET_ORGANIZATION/repository.git (push)
```

## 5. Push the mirror to the destination

```bash
git push --mirror
```

## 6. Verify the migration

Open the destination repository on GitHub and verify that all branches, tags, commits, and repository history have been transferred.
