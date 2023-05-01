- Exec commands below
```sh
$ pwd
/workspaces/custom-template-for-dotnet-new/samples/00-minimum-template

$ ls
README.md  SampleProject.00

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
   /workspaces/custom-template-for-dotnet-new/samples/00-minimum-template

Success: /workspaces/custom-template-for-dotnet-new/samples/00-minimum-template installed the following templates:
Template Name      Short Name  Language  Tags   
-----------------  ----------  --------  -------
Sample Project 00  sample00

$ dotnet new -l Sample
These templates matched your input: 'Sample'

Template Name      Short Name  Language  Tags   
-----------------  ----------  --------  -------
Sample Project 00  sample00

$ dotnet new sample00 --name sampleTest00
The template "Sample Project 00" was created successfully.

$ ls
README.md  SampleProject.00  sampleTest00

$ cd sampleTest01/

$ dotnet run
Date created: 2023/04/28

$ cd ..
$ rm -rf sampleTest01/
```