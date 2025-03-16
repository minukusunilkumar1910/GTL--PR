 Creating, submitting, and managing pull requests on GitHub involves several steps. Here's a detailed walkthrough of the entire process from forking a repository to merging a pull request:

1. Fork the Repository
Forking a repository creates a copy of the original repository in your GitHub account.

Go to the repository you want to contribute to.
Click on the "Fork" button at the top right of the repository page.

2. Clone the Forked Repository
Clone the forked repository to your local machine to start making changes.

sh
git clone https://github.com/<your-username>/<repository-name>.git
cd <repository-name>

3. Set Up the Upstream Remote
Set up the original repository as the upstream remote to keep your fork updated with changes from the main repository.

sh
git remote add upstream https://github.com/<original-owner>/<repository-name>.git


4. Create a New Branch
Create a new branch to work on your changes. It's a good practice to create a branch for each feature or bug fix.

sh
git checkout -b <branch-name>


5. Make Changes and Commit
Make the necessary changes to the code. Once done, stage and commit the changes.

sh
git add .
git commit -m "Description of the changes"

6. Push Changes to Your Fork
Push the changes to the new branch in your forked repository.

sh
git push origin <branch-name>

7. Create a Pull Request
Go to the original repository on GitHub.
Click on the "Compare & pull request" button that appears after pushing changes to your fork.
Fill out the pull request form with a title and description of your changes.
Click on "Create pull request".

9. Discuss and Update
The repository maintainers will review your pull request. They might request changes or ask questions. You can update your pull request by pushing new commits to the same branch.

10. Keep Your Branch Updated
Keep your branch updated with the latest changes from the upstream repository.

sh
git fetch upstream
git checkout <branch-name>
git merge upstream/main
Resolve any merge conflicts if they arise and push the updated branch to your fork.

10. Merging the Pull Request
Once your pull request is approved, it can be merged into the main branch of the original repository. This can be done by the repository maintainers or sometimes by you if you have the necessary permissions.

Go to the pull request page.
Click on the "Merge pull request" button.
Confirm the merge.
11. Clean Up
After the pull request is merged, you can delete the branch both locally and on your fork.

sh
git branch -d <branch-name>
git push origin --delete <branch-name>
Summary
Fork the repository.
Clone the forked repository.
Set up the upstream remote.
Create a new branch.
Make changes and commit.
Push changes to your fork.
Create a pull request.
Discuss and update as needed.
Keep your branch updated.
Merge the pull request.
Clean up branches.
This process ensures that your contributions are properly integrated into the main repository while allowing maintainers to review and manage changes effectively.
