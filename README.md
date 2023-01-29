# _PierreSweets.Solution_

#### By _**Oscar Gonzalez**_

#### _This is an app that lets you create a treat or a flavor to match; as well as a list for either of the two. You can then assign a treat to a specific flavor and vice versa. Each treat can have a list of flavors that are assigned to said treat, and a list of treats that have been assigned specific flavors. With that being said, the app only allows authenticated users to create, edit, or delete. An un-authenticated user can see a list of either treats or flavors, and each of the treats' and flavors' respective associations only after an authenticated user has created them._

## Technologies Used

* _C#_
* _.NET6_
* _HTML_
* _CSS_
* _Razor Markup_
* _MySQLWorkbench_
* _SQL Database_
* _AspNetCore_
* _Linq_
* _EntityFrameworkCore_
* _AspNetCore.Mvc_
* _AspNetCore.Mvc.Rendering_
* _AspNetCore.Identity_
* _AspNetCore.Authorization_
* _ViewBag_



## Description

_This is my twelfth project for Epicodus that is meant to show off my understanding of basic web applications with a database whilst utilizing C#; it is also meant to show my understanding of many-to-many relationships, and authentication with identity. Here is a [link](https://github.com/OLGON92/PierreSweets.Solution) to the repository on GitHub._

## Setup/Installation Requirements
* _Follow the steps below_

#### Installing .NET & MySQL
* _First, you will need to install .NET 6 if it isn't already on your machine_
* _Here is a link where you can download for your Mac, Windows, or Linux based machince: [link](https://dotnet.microsoft.com/en-us/download/dotnet/6.0)_
* _Look in your downloads and open the file_
* _Follow the installation intructions_
* _To confirm the the installation was a success: on your command line in your terminal type "dotnet --version"_
* _Then you will need to install MySQL. Follow the instructions in here[link](https://www.learnhowtoprogram.com/c-and-net/getting-started-with-c/installing-and-configuring-mysql) to do so._

#### Configuring appsettings.json
* _Clone the repository using this link: [link](https://github.com/OLGON92/PierreSweets.Solution)_
* _Navigate to the 'PierreSweets.Solution' directory on your computer_
* _Open it with your favorite text editor (Visual Studio Code is one I highly reccomend)_
* _From here you will go to the "PierreSweets" Directory_
* _Create a new file called "appsettings.json_
* _In the appsettings.json file you will add the following code below_
* _*Please note that your username and password is dependent on what you have set up in your MySQLWorkbench.*_
* _*Also, do not include the brackets []*_
```
{
  "ConnectionStrings": {
      "DefaultConnection": "Server=localhost;Port=3306;database=oscar_gonzalez;uid=[YOUR-USERNAME-HERE];pwd=[YOUR-PASSWORD-HERE];"
  }
}
```



#### To add a migration, start a development server, and view the project in the browser follow the steps below:_
* _Navigate to 'PierreSweets.Solution' in your command line_
* _From there navigate to 'PierreSweets'_
* _Run the command "dotnet build"_
* _Then run the command "dotnet tool install --global dotnet-ef --version 6.0.0"_
* _Then you will run the command "dotnet add package Microsoft.EntityFrameworkCore.Design -v 6.0.0"_
* _Now you will need to create a migration; run the command "dotnet ef migrations add Initial"_
* _Anytime you make a change to any of the models, you will have to enter this command "dotnet ef migrations add [ChangeInMigration]" . Please note that the brackets don't need to be there, and words in brackets are an example._
* _After verifying that the changes are correct enter "dotnet ef database update". If you would like to remove a migration, enter "dotnet ef migrations remove"_
* _Then run the command "dotnet watch run"_
* _It should then open the development environment in your preferred web browser automatically_
* _If it does not open automatically, then open your preferred web browser, copy/paste this http://localhost:5000 into your web browser, and you should be able to use the app after that_


#### To view your schema in MySQL Workbench follow the steps below
* _Open MySQLWorkbench, and click on the "Local instance 3306" box_
* _From here you will click on the "Schemas" tab on the left_
* _On the left you should see the name of the schema you created in the appsettings.json file_




## Known Bugs

* _None to be found._


## License

_If you have any questions or concerns please contact me at ogon318@gmail.com
You are also welcome to make any contributions if you'd like_

* _MIT License

Copyright (c) 2023 Oscar Gonzalez

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE._