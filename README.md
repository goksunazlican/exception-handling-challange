# exception-handling-challange
In this challenge, the task is to debug the existing code to successfully execute all provided test files.

I editted the `process_input` function as:

```cpp
void process_input(int n) {
    try{
        int d = largest_proper_divisor(n);
        cout << "result=" << d << endl;
        cout << "returning control flow to caller" << endl;

    }
    catch(const std::invalid_argument& ia){
        cout << ia.what() << endl;
        cout << "returning control flow to caller" << endl;
    }
        
}
```
