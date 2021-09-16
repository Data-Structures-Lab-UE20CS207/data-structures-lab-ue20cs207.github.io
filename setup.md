---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: post
title: Setup
permalink: /setup/
---

1. Do not remove this line (it will not be displayed)
{:toc}

&nbsp;
&nbsp;
&nbsp;

## Setup for Students

### Step 1: Setting up your GitHub accounts with PES email IDs (optional)

1. Create a [GitHub](https://github.com){:target="_blank"} Account with your MS Teams college email address (your email ID will be of the form **\<SRN\>@pesuonline.onmicrosoft.com** - check [PESU Academy](https://www.pesuacademy.com/Academy/){:target="_blank"} if you have forgotten)

2. Create a username of the form `SRN-firstname`, where SRN is in all caps and firstname is in all lowercase. For example, if your SRN is **PES1UG20CS001** and your name is **Aman**, your username must be `PES1UG20CS001-aman`

    <img src="/assets/images/SignUp.png" alt="SignUp" style="zoom:30%; display: block; margin-left: auto;  margin-right: auto;" />

3. Verify your account by checking your [email](https://outlook.office365.com){:target="_blank"} for the launch code

### Step 2: Joining a Classroom

1. For every assignment released, you will be given a GitHub classroom link.

2. Click on the link.

3. You will be asked to identify youself from a list of your SRNs. **Please do not skip this step**, as it is mandatory to link your GitHub account to your SRN. If this step is skipped, you will not be graded.

    <img src="/assets/images/Student_pov.png" alt="Student_pov" style="zoom:30%; display: block; margin-left: auto;  margin-right: auto;" />

4. Accept the assignment.

    <img src="/assets/images/Student_accept.png" alt="Student_accept" style="zoom:30%; display: block; margin-left: auto;  margin-right: auto;" />

&nbsp;
&nbsp;

## Setup for Teachers

### Step 1: Creating an Account on GitHub Classroom

1. Make sure you have a GitHub account that has been made an owner of the organisation [Data-Structures-Lab-UE20CS207](https://github.com/Data-Structures-Lab-UE20CS207). Please contact the TAs if you haven't been added.

2. Visit [GitHub Classroom](https://classroom.github.com/) and click on Sign In. You will be redirected to a page that looks like this. Sign in with the same GitHub account that has been added to the organisation.

    <img src="/assets/images/GitHub_classroom_sign_in.png" alt="GitHub_classroom_sign_in" style="zoom:30%; display: block; margin-left: auto;  margin-right: auto;" />

3. Once signed in, you should see a landing page with all your classrooms (empty for newly linked classroom accounts).

    <img src="/assets/images/GitHub_classroom_create.png" alt="GitHub_classroom_create" style="zoom:30%; display: block; margin-left: auto;  margin-right: auto;" />

### Step 2: Creating a New Classroom

Follow these steps if the TA's have not created a classroom for a section. If this process has been done already, skip to [Creating an assignment](#create-assignment).

1. Click on the "Create your first classroom" button. If your account has been added to the organisation correctly, you should see the **Data-Structures-Lab-UE20CS207** organisation.

    <img src="/assets/images/GitHub_classroom_create_new.png" alt="GitHub_classroom_create_new" style="zoom:30%; display: block; margin-left: auto;  margin-right: auto;" />

2. Select the organisation **Data-Structures-Lab-UE20CS207**. You will be asked to name the classroom. Please follow the naming convention **Data-Structures-Lab-UE20CS207-\<class\>-\<capital_section\>**. For example, to create a classroom for 3A, name the classroom **Data-Structures-Lab-UE20CS207-3-A**. For the demo here, a classroom called **Data-Structures-Lab-UE20CS207-3-Z** has been created.

    <img src="/assets/images/GitHub_classroom_name.png" alt="GitHub_classroom_name" style="zoom:30%; display: block; margin-left: auto;  margin-right: auto;" />

3. Once successfully created, you will be taken to a "Success" page. If you have other collaborators (teachers, TAs) helping with **this class**, make sure that they are admins of the GitHub organisation and then copy the link of the classroom and send it to them personally.

    <img src="/assets/images/GitHub_collab.png" alt="GitHub_collab" style="zoom:30%; display: block; margin-left: auto;  margin-right: auto;" />

4. The final step in creating a classroom is to add a list of students mapped to their SRNs.

    <img src="/assets/images/GitHub_classroom_roster.png" alt="GitHub_classroom_roster" style="zoom:30%; display: block; margin-left: auto;  margin-right: auto;" />

    Since PES does not use a Learning Management System to manage all the students, scroll down to the bottom of the page and upload a CSV of all the students in your classroom. Once uploaded, the names and SRNs should show up in the text box.

    <img src="/assets/images/GitHub_classroom_names.png" alt="GitHub_classroom_names" style="zoom:30%; display: block; margin-left: auto;  margin-right: auto;" />

    If successful, you should be taken to the classroom's home page.

    <img src="/assets/images/GitHub_classroom_home.png" alt="GitHub_classroom_home" style="zoom:30%; display: block; margin-left: auto;  margin-right: auto;" />

### Step 3: Creating an Assignment
{: #create-assignment}

#### Create template repository with starter code

1. The first step is to create a template repository on GitHub with the template code for the assignment. To do that, go to the organisation's homepage [here](https://github.com/Data-Structures-Lab-UE20CS207) and create a new repository.

    Once you have created your template code, push it to any public GitHub repository (or a repository on the organisation; preferable). This can be done by running 

    ```bash
    git init
    git branch -m main
    git remote add origin <repo_url>
    ```

    Verify that the remote has been added by running
    
    ```bash
    git remote -v
    ```

    Commit and push the changes to the remote repo (after pulling)

    ```bash
    git pull origin main
    git add .
    git commit -m "Your commit message"
    git pish origin main
    ```

    Note that any testing scripts that are on the repository will not be hidden frm the students, and will be considered to be sample test cases.

2. Convert the repository with the template code into a template repository. Go to the repository on GitHub and click on the settings tab. If you can't see settings, click on the three dots.

    <img src="/assets/images/GitHub_settings.png" alt="GitHub_settings" style="zoom:30%; display: block; margin-left: auto;  margin-right: auto;" />

    Go to the Options tab, and select the checkbox for "Template repository".

    <img src="/assets/images/GitHub_template.png" alt="GitHub_template" style="zoom:30%; display: block; margin-left: auto;  margin-right: auto;" />

#### Create assignment on GitHub Classroom

1. Go to GitHub classroom and click on "Create an assignment". Give it an appropriate title, deadline, and select "Individual assignment". **Ensure that you select Private for Repository visibility**, as failing to do so will allow the students' code to be publicly visible. Do not grant students admin access to their repositories.

    <img src="/assets/images/GitHub_classroom_basics.png" alt="GitHub_classroom_basics" style="zoom:30%; display: block; margin-left: auto;  margin-right: auto;" />

2. Add the template repository previously created as the starter code template.

    <img src="/assets/images/GitHub_classroom_search_template.png" alt="GitHub_classroom_search_template" style="zoom:30%; display: block; margin-left: auto;  margin-right: auto;" />

3. Optionally, add VS code as a supported editor (recommended).

    <img src="/assets/images/GitHub_editor.png" alt="GitHub_editor" style="zoom:30%; display: block; margin-left: auto;  margin-right: auto;" />


#### Add autograding

1. Testing with the test scripts (sample tests) visible to the students (test.sh) - add a "Run command" test. You can award points as required.

    <img src="/assets/images/Test_1.png" alt="Test_1" style="zoom:30%; display: block; margin-left: auto;  margin-right: auto;" />

2. Hidden test cases: run Input/Output tests.

    <img src="/assets/images/Test_2.png" alt="Test_2" style="zoom:30%; display: block; margin-left: auto;  margin-right: auto;" />


    For more on autograding, read [this](https://docs.github.com/en/education/manage-coursework-with-github-classroom/teach-with-github-classroom/use-autograding#inputoutput-test)

4. Create the assignment and copy the invitation URL. Send it to all students either via Edmodo, email or for the TAs to update the portal.

    <img src="/assets/images/GitHub_created.png" alt="GitHub_created" style="zoom:30%; display: block; margin-left: auto;  margin-right: auto;" />
