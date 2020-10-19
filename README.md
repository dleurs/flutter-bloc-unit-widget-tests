# Flutter CICD with test package (unit and widget tests), BLoC pattern, Gitlab and FastLane
![Counter App](/assets/CounterApp.png)<br/>

Using <strong>bloc_test package </strong><br/>

On VSCode, click on Run inside /test/test_counter_bloc.dart, near main(), to launch bloc tests<br/>
![Run Button](/assets/RunButton.png)<br/>

See below successful logs<br/>
![Logs In Case Of Success](/assets/LogsInCaseOfSuccess.png)<br/>

Difficulties :
- InitialCounterState seems to not be create when CounterBloc()
- flutter test does not launch test_counter_bloc.dart
- Why creating a mock :
```dart
class MockCounterBloc extends MockBloc<CounterState> implements CounterBloc {}
```

Documentation :<br/>
https://pub.dev/packages/bloc_test/example

https://github.com/felangel/bloc/tree/master/packages/bloc_test

https://medium.com/flutter-community/unit-testing-with-bloc-b94de9655d86

https://www.youtube.com/watch?v=S6jFBiiP0Mc

https://pub.dev/packages/bloc_test