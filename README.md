# HandsOnWebApp

In this application, you are tasked with implementing a backend using either NestJs with Express or .NET; the choice is yours. Optionally, you may use [NX](https://nx.dev/) to build a monorepo and segregate the application from the web API within the same repository. Additionally, develop a frontend app using Angular or NextJs. Focus on functionality rather than aesthetics for the layout. 

## App should have three screens:

  - **Main**: Displays a list of jobs, preferably paginated. Each job is clickable and redirects to the job screen.
  - **Job**: Shows the job description along with a button to apply.
  - **Apply**: Contains a form to apply for a job. Here, applicants must input their name and email and provide some text about their application. After submitting the application, an email should be sent to the company using this simulated SMTP server: [Ethereal Email](https://ethereal.email/).

## API with three controllers:
  - **Company**: Operations include listing companies, adding a company, and removing a company.
  - **Job**: Functions to add a job, list jobs, and remove a job.
  - **Appliances**: Handles job applications.

## Communication between database and API:
 - Utilize an ORM; options include MikroOrm, TypeORM, or EF (Entity Framework) if using .NET.
 - Implement a repository layer for data fetching.

## Two database tables:
  - **Appliances**:
    - Job id;
    - User Name;
    - User Email;
    - Appliance text.
  - **Job**:
    - Job id;
    - Job name;
    - Job description;
    - Company name (must be unique to prevent duplicate entries).

**Use interfaces whenever it's possible or you feel like you should have them**
**Although all aspects have their own weigh, we pay special attention in the way the code base is structured as a whole**
