### Examples of Flutter State Management through BLoC and Cubits

1. todo app -> cubit
2. login page -> bloc
3. weather -> bloc and feature first dir organisation.

### Notes:
1. Bloc builder listens to emits and changes in state to render componenent accordingly.
2. Bloc listener listens to emits and changes in state to execute some function like Navigation etc.
3. Bloc Consumer = Bloc Listener + Bloc builder.
4. Cubit only stores state in class and emit's can be triggered outside the cubit by directly calling the state change functions with adding any event listener to widget.
5. Bloc has events and states, and events are added to components. These events can emit state change but only from inside the BLoC not anywhere outside.
6. Bloc Observer is a midlleware we can add to see the state change and transitions for ease in debugging.

### Layers for effective Bloc management
- Presentation Layer -> Screens and Widgets
    |
- BLoc layer -> For state management
    |
- Repository layer -> The datat recieved is formated to data models
    |
- Network layer -> Interacts with other exerternal APIs for data
