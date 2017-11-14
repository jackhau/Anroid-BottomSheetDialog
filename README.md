# Bottom Sheet Dialog Example
A simple library that creates BottomSheets according to the Material Design

# Screenshots
![1213](https://user-images.githubusercontent.com/13564867/32759261-6ce70698-c923-11e7-9ca1-f6b3a005979f.jpg)
![1213](https://user-images.githubusercontent.com/13564867/32759277-80e03318-c923-11e7-86af-aaddeadf84e1.jpg)


- Add the following to your build.gradle:
```groovy
dependencies {
  compile 'com.android.support:design:25.3.1'
  compile 'com.android.support:appcompat-v7:25.3.1'
}
```

- Create a BottomSheetMenuDialog:
```java
    ButtomDialog buttomDialog = new ButtomDialog(MainActivity.this);
    buttomDialog.show();
```

```java
public class ButtomDialog extends BottomSheetDialog {

    public ButtomDialog(@NonNull Context context) {
        super(context);
    }

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(getLayoutInflater().inflate(R.layout.dialog_layout, null));
        getWindow().setLayout(LinearLayout.LayoutParams.MATCH_PARENT, LinearLayout.LayoutParams.WRAP_CONTENT);
    }
}
```
