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
      <input type="text" #title>        
        @ViewChild('title') 
        private elTitle : ElementRef; 
      we will use multiple @ViewChild() in parent component. 
     
  # Renderer2 
  
    It is used for UI rendering manipulation. Using Renderer2, we can create element, provide a text and then it can be appended with any existing element at run time on any event of an element.
    
    We can add and remove CSS classes, styles, HTML attributes using Renderer2 to change the UI. We can also set DOM property with a value at run time using Renderer2.
    
    We can append and remove a child element within a parent element using Renderer2. It can also be used to add a HTML comment to a given parent element. We can also bind an element to listen event using Renderer2.
