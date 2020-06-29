## Model-View-ViewModel (MVVM)

Is a _code organizing_ architectural design paradigm, which works in concert with the concept of "reactive" user-interfaces.

> On MVVM paradigm we try to separate the Model and the View.

### Model
The *Model* is UI independent, it encapsulates *the data and logic* of your application. The model is the _Truth_.

### View
The *View* reflects the model (_stateless_), the data is always flowing from the model to the view. The view is stateless because it takes the existing state of the mode and them displays it. 

The view is *declarative*, it means that we declare that the view looks a certain way and only change when the model changes. The view needs also to be *reactive*, which means that each time the Model changes the view needs to respond the changes.

### ViewModel

The ViewModel's job is to bind the view to the Model, interpert the model to the view. The view model always awaits for changes on the model and then interpert the changes if needed, lastly it publishes the changes to the view. The view subscribes to the interpeter and looks to know when something changes. The ViewModel can also process intent, when we want our ui View to request the Model do process a change, once the Model is changed it sends back the notification to modify the View.

