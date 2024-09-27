# Version Control Systems: Git

## What is Git?
Git is a distributed version control system that allows multiple developers to collaborate on the same codebase efficiently. It tracks changes to files, enabling teams to work simultaneously while maintaining the integrity of the code.

### Key Features of Git
- **Branching**: Allows developers to create independent lines of development, known as branches. 
- **Merging**: Combines code changes from different branches.
- **History**: Git maintains a full history of changes, allowing you to revert to previous versions if necessary.

### Common Git Commands
- `git clone`: Clone a repository.
- `git add`: Stage changes for a commit.
- `git commit`: Save your changes to the repository.
- `git push`: Send commits to a remote repository.
- `git pull`: Fetch and merge changes from a remote repository.

### Branching Strategies
1. **Feature Branches**: Every feature or bug fix is developed in its own branch.
2. **GitFlow**: A workflow where master and develop branches are maintained alongside feature and release branches.
3. **Trunk-Based Development**: A simpler workflow where all developers commit to a single mainline (trunk) branch, with frequent merges.

### Code Reviews with Git
Code reviews are a critical practice in DevOps, where peers review each other’s changes to ensure quality and correctness.

- **Pull Requests**: When a developer wants to merge changes, they submit a pull request, which is then reviewed by their peers.
- **Merge Conflicts**: Occur when two developers edit the same part of a file in conflicting ways. Resolving conflicts ensures the final codebase is consistent.

### Example Workflow
1. Create a new branch for a feature: `git checkout -b new-feature`.
2. Make changes and commit: `git add . && git commit -m "Implemented new feature"`.
3. Push changes to the remote: `git push origin new-feature`.
4. Create a pull request for peer review.
5. Merge the branch once approved: `git merge new-feature`.
