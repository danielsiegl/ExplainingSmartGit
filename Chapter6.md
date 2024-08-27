# Chapter 6: Step by Step GitHub Flow

## Summary
We use GitHub Flow as a relatively simply best practice workflow that works great with modern Git environments. See the official documentation: https://docs.github.com/en/get-started/using-github/github-flow

## Initial git repository creation

```mermaid
---
title: Initial git repository creation
---
gitGraph
   commit
   commit
```

## Create feature branch

```mermaid
---
title: Create feature branch
---
gitGraph
   commit
   commit
   branch feature1
   checkout feature1
   commit type: HIGHLIGHT
```

## Work on feature branch

```mermaid
---
title: Create feature branch
---
gitGraph
   commit
   commit
   branch feature1
   checkout feature1
   commit type: HIGHLIGHT
   commit type: HIGHLIGHT
   commit type: HIGHLIGHT
   commit type: HIGHLIGHT
```

## Others bring change to the main branch

```mermaid
---
title: Others bring change to the main branch
---
gitGraph
   commit
   commit
   branch feature1
   checkout feature1
   commit
   commit
   checkout main
   commit type: HIGHLIGHT
   commit type: HIGHLIGHT
   checkout feature1
   commit
```

## Review changes

```mermaid
---
title: Others bring change to the main branch
---
gitGraph
   commit
   commit
   branch feature1
   checkout feature1
   commit
   commit
   checkout main
   commit
   commit
   checkout feature1
   commit
   commit id: "Changes after review" type: HIGHLIGHT
```

## Merge changes back to main

```mermaid
---
title: Merge changes back to main
---
gitGraph
   commit
   commit
   branch feature1
   checkout feature1
   commit
   commit
   checkout main
   commit
   commit
   checkout feature1
   commit
   commit id: "Changes after review"
   checkout main
   merge feature1 id: "merge"
```

## Our changes are now included in the new mainline

```mermaid
---
title: Merge changes back to main
---
gitGraph
   commit
   commit
   branch feature1
   checkout feature1
   commit
   commit
   checkout main
   commit
   commit
   checkout feature1
   commit
   commit id: "Changes after review"
   checkout main
   merge feature1 id: "merge" tag: "All changes" type: HIGHLIGHT
```
