# Capstone Project: Enhancing a Community Library Website

### Steps taken to complete tasks:

### Setup

1. Create a Repository on GitHub:
+ Name it greenwood-library-website
+ Make sure to make the repository public
+ Initialize it with a README.md file and clone it to your local machine

![GitHub_Repo_Clone_1](/Capstone_Project_Git/Images/GitHub_Repo_Clone_1.png)

![GitHub_Repo_Clone_2](/Capstone_Project_Git/Images/GitHub_Repo_Clone_2.png)



### Tasks: Steps

1. Create files for the home.html, about_us.html, events.html and contact_us.html by using the following command

```
touch home.html about_us.html events.html contact_us.html
```
+ Check that files are created by using the following command:
```
ls
```

![Create_webpage_files](/Capstone_Project_Git/Images/Create_webpage_files.png)

2. Add random content into each of the files created

![Adding_content_to_home.html](/Capstone_Project_Git/Images/Adding_content_to_home.html.png)

![Adding_content_to_About_Us.html](/Capstone_Project_Git/Images/Adding_content_to_About_Us.html.png)

![Adding_content_to_Events.html](/Capstone_Project_Git/Images/Adding_content_to_Events.html.png)

![Adding_content_to_Contact_Us.html](/Capstone_Project_Git/Images/Adding_content_to_Contact_Us.html.png)

3. Stage, commit and push the changes directly to the main branch by issuing the following commands:

   **Staging**

   Check the status of changes made by using this command:
   ```
   git status
   ```
   Then stage the changes to be committed by using the following command:
   ```
   git add .
   ```
   ![Main_Staging](/Capstone_Project_Git/Images/Main_Staging.png)

   **Committing changes**

   Commit changes made by issuing the following command:
   ```
   git commit -m "Base Content for Website"
   ```
   ![Main_Commit_Push](/Capstone_Project_Git/Images/Main_Commit_Push.png)

   **Pushing committed changes**

   Push committed changes to Main branch by issuing this command:
   ```
   git push origin main
   ```
   ![Main_Commit_Push](/Capstone_Project_Git/Images/Main_Commit_Push.png)

   
### Morgan's Work: Adding Book Reviews

### Steps to Adding Book Reviews

1. Create a branch for Morgan by:

   + Creating a new branch and Switching to it (There are two options to doing this; first is by creating the branch and then switching to it. Second is creating the new branch and switching to it at the same time. We will go with the first option for this task)
   + Create new branch by issuing the following command:
     ```
     git branch add-book-reviews
     ```

   + Switch to new created branch by issuing the following command:
     ```
     git switch add-book-reviews
     ```

   ![Book_Reviews_branch_Switching](/Capstone_Project_Git/Images/Book_Reviews_branch_Switching.png)

2. Add a new file book_reviews.html to represent the Book Reviews Section by issuing the following command:
   ```
   touch book_reviews.html
   ```

3. Add random text content into the file by using the following command:
   ```
   vi book_reviews.html
   ```
   + Add content as desired
   
   ![Content_Book_Reviews_Page](/Capstone_Project_Git/Images/Content_Book_Reviews_Page.png)

4. Stage, Commit and Push Changes by issuing the following commands:

   + Staging changes:
     ```
     git status
     ```
     ```
     git add .
     ```
     ![Book_Reviews_Staging](/Capstone_Project_Git/Images/Book_Reviews_Staging.png)

   + Committing changes:
     ```
     git commit -m "Add book reviews section"
     ```
     ![Book_Reviews_Commit](/Capstone_Project_Git/Images/Book_Reviews_Commit.png)

   + Pushing changes:
     ```
     git push origin add-book-reviews
     ```
     ![Book_Reviews_Push](/Capstone_Project_Git/Images/Book_Reviews_Push.png)
     
5. Raise a Pull Request (PR) for Morgan's work by doing the following:

   + Creating a pull request from the GitHub Repository
     ![Book_Reviews_PR](/Capstone_Project_Git/Images/Book_Reviews_PR.png)

6. Merge Morgan's work to the main branch by doing the following:

   + Confirming to merge the pulled content from Morgan's branch into the Main branch
     ![Book_Reviews_Merge_1](/Capstone_Project_Git/Images/Book_Reviews_Merge_1.png)

     ![Book_Reviews_Merge_2](/Capstone_Project_Git/Images/Book_Reviews_Merge_2.png)

   
### Jamie's Work: Updating Events Page

### Steps to Updating Events Page

1. Create a branch for Jamie and switch to it by:
   
   + Creating a new branch and Switching to it (There are two options to doing this; first is by creating the branch and then switching       to it. Second is creating the new branch and switching to it at the same time. We will go with the second option for this task)
   + Create and swith to a new branch by issuing the following command:
     ```
     git checkout -b update-events
     ```

   ![Creating_Update_events_Switching_To_it](/Capstone_Project_Git/Images/Creating_Update_events_Switching_To_it.png)

2. Add updated text content into the events.html file by using the following command:
   ```
   vi events.html
   ```

   ![Updated_Events.html_1](/Capstone_Project_Git/Images/Updated_Events.html_1.png)

   ![Updated_Events.html_2](/Capstone_Project_Git/Images/Updated_Events.html_2.png)

3. Stage, Commit and Push Changes by issuing the following commands:

   + Staging changes:
     ```
     git status
     ```
     ```
     git add .
     ```
     ![Update_events_Staging](/Capstone_Project_Git/Images/Update_events_Staging.png)

   + Committing changes:
     ```
     git commit -m "Update to events section"
     ```
     ![Updated_events_Commit](/Capstone_Project_Git/Images/Updated_events_Commit.png)

   + Pushing changes:
     ```
     git push origin update-events
     ```
     ![Updated_events_Pushing](/Capstone_Project_Git/Images/Updated_events_Pushing.png)

4. Pull the latest changes from the main branch into update-events by issuing the following command:
   ```
   git pull origin main
   ```
   ![Pull_Changes_To_update_events](/Capstone_Project_Git/Images/Pull_Changes_To_update_events.png)

5. Raise a Pull Request (PR) for Jamie's work by doing the following:

   + Creating a pull request from the GitHub Repository
     ![Update_events_PR_1](/Capstone_Project_Git/Images/Update_events_PR_1.png)

     ![Update_events_PR_2](/Capstone_Project_Git/Images/Update_events_PR_2.png)

6. Merge Jamie's work to the main branch by doing the following:

   + Confirming to merge the pulled content from Morgan's branch into the Main branch
     ![Update_events_Merge_1](/Capstone_Project_Git/Images/Update_events_Merge_1.png)

     ![Update_events_Merge_2](/Capstone_Project_Git/Images/Update_events_Merge_2.png)

     ![Update_events_Merge_3](/Capstone_Project_Git/Images/Update_events_Merge_3.png)
     
