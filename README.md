# Webapp migration to Angular 10

The purpose of this repo is to track issues, bugs, todos, and anything else that might be related to the Angular 10 migration. 

Quick links:
- This is the [branch](https://github.com/medic/cht-core/tree/4750-angular-10-take-2) that devs are working on. This branch is not stable, as PRs are merged before passing through quality-assurance acceptance testing.    
- This is the [progress spreadsheet](https://docs.google.com/spreadsheets/d/13BBw8cyV8CLMOzZAR_WDBqkaNrywNOk-i7b7pcypWJ8/edit#gid=0) where devs assign themselves to migrate files. 

### [Project Board](https://github.com/medic/angular10-migration/projects/1)

Please use this [project board](https://github.com/medic/angular10-migration/projects/1) to track issues.   
Please follow the same guidelines related to assigning and moving issues around in columns as you do in CHT-Core release project boards. 

### Updated Libraries

| Description | Old | Migration | New | 
| ------ | --- | --- | --- | 
| framework | [AngularJS 1.7](https://angularjs.org/) | Replacement | [Angular 10](https://angular.io/) | 
| navigation | [ui-router](https://github.com/angular-ui/ui-router) | Replacement | [Angular 10 builtin router](https://angular.io/api/router/Router) | 
| cookie helper | [angular-cookie](https://www.npmjs.com/package/angular-cookie) | Replacement | [ngx-cookie-service](https://www.npmjs.com/package/ngx-cookie-service) | 
| translations | [angular-translate](https://github.com/angular-translate/angular-translate) | Replacement | [@ngx-translate/core](https://github.com/ngx-translate/core) | 
| bootstrap | [Bootstrap 3.4](https://getbootstrap.com/docs/3.4/getting-started/) | | [Bootstrap 3.4](https://getbootstrap.com/docs/3.4/getting-started/) but no longer used directly in templates but via ngx-bootstrap |
| bootstrap helper | [angular ui-bootstrap](https://angular-ui.github.io/bootstrap/) | Replacement | [ngx-bootstrap](https://valor-software.com/ngx-bootstrap/#/) | 
| redux | [redux](https://www.npmjs.com/package/redux) and [ng-redux](https://github.com/angular-redux/ng-redux) and [redux-thunk](https://github.com/reduxjs/redux-thunk)| Replacement | [@ngrx/store](https://ngrx.io/guide/store) and [@ngrx/effects](https://ngrx.io/guide/effects) |
| redux logger | [redux-logger](https://github.com/LogRocket/redux-logger) | Replacement | [ngrx-store-logger](https://www.npmjs.com/package/ngrx-store-logger) | 
| pouchdb wrapper | [angular-pouchdb](https://www.npmjs.com/package/angular-pouchdb) | Removal | Using [NgZone](https://angular.io/api/core/NgZone) to enable change detection when interacting with PouchDB | 
 
