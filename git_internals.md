# Git Internals

Git works as a content-addressable storage system where everything is stored using hashes.

---

## Blob

A blob stores the content of a file. It does not store the file name, only the data.

---

## Tree

A tree represents a directory structure. It links file names to blobs and other trees.

---

## Commit

A commit points to a tree and contains metadata such as author, timestamp, and parent commit.

---

## HEAD

HEAD is a reference pointer to the current branch or commit. It determines where new commits will be added.

---

## Hashing

Git uses hashing (SHA-1 or SHA-256) to uniquely identify every object. This ensures data integrity and fast lookups.

---

## Staging Area (Index)

The staging area is where changes are stored before creating a commit. It acts as a buffer between the working directory and the repository.

---

## Data Flow

Working Directory → Staging Area → Repository

* Modify files
* Stage using `git add`
* Commit using `git commit`
