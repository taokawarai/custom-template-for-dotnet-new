- Exec commands below
```sh
$ pwd
/workspaces/custom-template-for-dotnet-new/samples/01-basic-template

$ ls
README.md  SampleProject.01  

$ dotnet new -l
These templates matched your input: 

Template Name                                 Short Name      Language    Tags                      
--------------------------------------------  --------------  ----------  --------------------------
ASP.NET Core Empty                            web             [C#],F#     Web/Empty                 
ASP.NET Core gRPC Service                     grpc            [C#]        Web/gRPC  
:
:

$ dotnet new -i ./
The following template packages will be installed:
   /workspaces/custom-template-for-dotnet-new/samples/01-basic-template

Success: /workspaces/custom-template-for-dotnet-new/samples/01-basic-template installed the following templates:
Template Name      Short Name  Language  Tags   
-----------------  ----------  --------  -------
Sample Project 01  sample01    [C#]      Console

$ dotnet new -l Sample
These templates matched your input: 'Sample'

Template Name      Short Name  Language  Tags   
-----------------  ----------  --------  -------
Sample Project 01  sample01    [C#]      Console

$ dotnet new sample01 --name sampleTest01
The template "Sample Project 01" was created successfully.

$ ls
README.md  SampleProject.01  sampleTest01

$ cd sampleTest01/

$ dotnet run
Date created: 2023/04/28

$ cd ..
$ rm -rf sampleTest01/
```