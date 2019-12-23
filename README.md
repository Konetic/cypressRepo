# cypressRepo
open terminal/command prompt
create a directory with: mkdir fileName
Cd to that fileName/folder in the directory to the local machine
initialize with npm init
then give description, author name, package name, git
install cypress: Npm install cypress
enter: ./node_modules/.bin/cypress open
The cypress window opens up
open with the folder with Visual Studio code
go to cypress folder and to get integration
then to examples
hover over and click New File icon
named sample.spec.js
type codes as follows to test GitHub login with incorrect credentials
describe("log into GitHub account with incorrect credentials", () =>{

    it("Navigate to GitHub website with incorrect credentials: userNmae and password", () => {

cy.visit("https://github.com/login")
cy.get('#user\[login\]').type("incorrectUserName")
cy.get("#btn btn-primary btn-block").click()

    })
})
then failed to login to
