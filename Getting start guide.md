Regular Angular

> npm install @angular/cli -g
> ng new proj-name --style=scss --routing (will put a router by default)
> ng serve


Cli-Helpers

ng generate component my-new-component
ng g component my-new-component # using the alias

# components support relative path generation
# if in the directory src/app/feature/ and you run
> ng g component new-cmp
# your component will be generated in src/app/feature/new-cmp
# but if you were to run
> ng g component ./newer-cmp
# your component will be generated in src/app/newer-cmp
# if in the directory src/app you can also run
> ng g component feature/new-cmp
# and your component will be generated in src/app/feature/new-cmp

Angular Universal

recommanded node version : 8.1.0

use the right cli
    > npm remove -g @angular/cli
    > npm install -g @angular/cli@1.4.10
    > ng --version
      @angular/cli: 1.4.10

npm install @angular/cli -g
ng new project-name --style="scss" --routing
downgrade in the package.json to angular4 if its higher
cd project-name
npm install --save @angular/platform-server
npm install --save @angular/animations
            npm i --save ajv-keywords (if needed)
remove node_modules folder
remove all the "^" from package.json
npm i

for npm errors
	update => > npm i npm -g
		then re-install cli
	> npm uninstall -g angular-cli
	> npm cache clear --force
	> npm install -g @angular/cli
		if its still has a problem..
	> npm install --save angular-common
	> npm install --save rxjs



in app.module.ts change
BrowserModule.withServerTransition({appId: 'itunes-ng5'})
add app.server.module.ts file
copy the server.ts to the src folder
update the tsconfig.app.json (add server.ts) and tsconfig.json (add angularCompilerOptions)
update the package.json file (in the script)

> npm run start


