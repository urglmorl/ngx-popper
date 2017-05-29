# ngx-popper  

ngx-popper is an angular wrapper for the [popperjs](https://popper.js.org/).

### Installation

node and npm are required to run this package.

1. Use npm to install the package

  ```terminal
  $ npm install ngx-popper --save 
  ```

2. You could either add into your module `imports` the `NgxPopperModule` in order to add all of the pipes, Or add a specific module such as `NgArrayPipesModule`, `NgObjectPipesModule`, `NgStringPipesModule`, `NgMathPipesModule` or `NgBooleanPipesModule`.

  ```typescript
  import {NgxPopperModule} from 'ngx-popper';
  
  @NgModule({
   // ...
   imports: [
     // ...
     NgxPopperModule
   ]
  })
  ```

3. Add to view

  ```HTML  
   <div #popper1
            [popper]="popper1Content"
            [popper-show-onstart]="true"
            [popper-trigger]="'click'"
            [popper-placement]="'bottom'">
         <p class="bold">Hey!</p>
         <p class="thin">Choose where to put your popper!</p>         
       </div>
       <popper-content #popper1Content>
         <p class="bold">Popper on bottom</p>
       </popper-content>
  ```

### Demo
<a href="https://mrfrankel.github.io/ngx-popper/">Demo</a>

### Contribute
 
    terminal
      $ yarn install
      $ npm run dev 
      


