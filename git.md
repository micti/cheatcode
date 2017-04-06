# ``git cherry-pick`` - Bring code to all branches.

    master   A -> B -> C -> D
              \
    feat       -> E -> F
  
D -> feat
 
    git checkout feat
    git cherry-pick D
  
Result
 
    master   A -> B -> C -> D
              \
    feat       -> E -> F -> D' (D' = D)

C D -> feat

    git checkout feat
    git cherry-pick C D
  
Result
 
    master   A -> B -> C -> D
              \
    feat       -> E -> F -> C' -> D' (C' = C, D' = D)
    
More
 
- Git document: https://git-scm.com/docs/git-cherry-pick
- Don't forget ``git rebase`` :)

# ``git log`` List commits

    git log --pretty=oneline
    git log --pretty=format:"%h : %s"
