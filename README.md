# Jigsaw Solver
This is a simple Jigsaw solver (and creator) that works on any real image. (Computer generated images deliberately designed to fool the solver may give poor results)

# Explanation

Given an input jigsaw (images split into square blocks that are shuffled around), the solver solves the puzzle in 3 stages.

![jigsaw-process](https://user-images.githubusercontent.com/30972152/105203353-0647e200-5b69-11eb-97b8-5620d7ca13fa.png)

# LP Formation

![finding-weights](https://user-images.githubusercontent.com/30972152/105204645-6a1eda80-5b6a-11eb-8519-e1915ddadc37.png)

![solving-puzzle](https://user-images.githubusercontent.com/30972152/105204851-933f6b00-5b6a-11eb-83ac-39ae93006854.png)

## Greedy Filling
Since the LP does not contain any constraint to prevent collision among two pieces or a position remaining unoccupied. We must use some other technique to complete the solution.
In this case we employ Greedy Filling technique described by Gallagher \[2\]

## References

1. Yu, R., Russell, C., & Agapito, L. (2015). Solving jigsaw puzzles with linear programming. arXiv preprint arXiv:1511.04472
2. Gallagher, A. C. (2012, June). Jigsaw puzzles with pieces of unknown orientation. In 2012 IEEE Conference on Computer Vision and Pattern Recognition (pp. 382-389). IEEE.
