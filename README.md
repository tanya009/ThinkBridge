# Application Setup

## **Angular Setup**

1. Clone the Angular project into any convinient folder in your system.
2. Open command line inside the angular folder and run the following command to install depndencies.

    ```
    npm install
    ```

3. Once the packages are installed, run the application with following command.

    ```
    ng serve
    ```

## **SQL Setup**

1. Install SQL Management studio and SQL Server if not already installed.
2. Create a local SQL Server instance if not already created.
3. Connect to the local SQL Server instance with SQL Management Studio.
4. Once conected, right click on the instance displayed in left partition of the Management studio and click on create new Database and provide the name as **Shop**.
5. Once created, open a new sql window and run the followiing command for table creation:

    ~~~~sql
    USE [Shop]
    GO

    SET ANSI_NULLS ON
    GO

    SET QUOTED_IDENTIFIER ON
    GO

    CREATE TABLE [dbo].[ShopB](
        [Name] [nvarchar](50) NOT NULL,
        [Description] [nvarchar](max) NULL,
        [Price] [nvarchar](max) NULL,
    CONSTRAINT [PK_ShopA] PRIMARY KEY CLUSTERED 
    (
        [Name] ASC
    )WITH (PAD_INDEX = OFF, STATISTICS_NORECOMPUTE = OFF, IGNORE_DUP_KEY = OFF, ALLOW_ROW_LOCKS = ON, ALLOW_PAGE_LOCKS = ON, OPTIMIZE_FOR_SEQUENTIAL_KEY = OFF) ON [PRIMARY]
    ) ON [PRIMARY] TEXTIMAGE_ON [PRIMARY]
    GO
    ~~~~

6. The database setup is complete.

## **.Net Application Setup**

1. Clone the .Net application form git to any convinient folder in your system.
2. Once cloned or downloaded, open the solution file in **_Visual Studio_** or any other suitable IDE and build the project.
3. Once the Build is succeeded, and provided the SQL server is up, the application is ready to run.

<br/>

### _The setup is done. Provided that all setup went as expected and the applications are up and running, kindly hit http://localhost:4200 to test the application._
