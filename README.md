# Angular-Basic-

# @ViewChild()
   It's used to configure a view query. It can be used to get the first element or the directive matching the selector from the view DOM.
   It provides the instance of another component or directive in parent component and then parent component can access the methods and properties of that component or directive. 
   In a parent component we can use @ViewChild() for components, directives and template reference variable with ElementRef or TemplateRef.
   To use @ViewChild() we need to pass child component name or directive name or template variable as an argument. 
   EX:  I have a component named as EmployeeComponent then within a parent component, we use it as follows,
   
  #  @ViewChild(EmployeeComponent)
  #  private employeeComponent: EmployeeComponent;
    The selector of the EmployeeComponent will be used in  parent component HTML template.
    
   EX: Directives using @ViewChild
     # @ViewChild(ColorDirective)
     # private colorDirective: ColorDirective;
     The selector name of directive CpColorDirective will be used in host element of DOM layout in parent component HTML template. 
     
  EX: Template Reference
      # <input type="text" #title>          --------parent component
      #  @ViewChild('title') 
      #   private elTitle : ElementRef; 
      we will use multiple @ViewChild() in parent component. 
     
