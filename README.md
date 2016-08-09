# LIVETemplate
Live Template for Android Studio

<b>Path:</b>
```
USER_PROFILE\.AndroidStudio***\config\templates
```
# Methods:

* cmvp - Check mvp view for null
``` java
    if(getMvpView() != null){
        
    }
```

* sa0 - Create startActivity() static method in Activity class; 
* sa1 - /---/ create with one arguments
* sa2 - /---/ create with two arguments
```java
    private static final String KEY_TEST_ID = "KEY.TEST_ID";

    public static void startActivity(Context context, String testId) {
        context.startActivity(getIntent(context, testId));
    }

    public static Intent getIntent(Context context, String testId) {
        Intent intent = new Intent(context, MvpFunctionPresenter.class);
        intent.putExtra(KEY_TEST_ID, testId);
        return intent;
    }
```

* fi0 - Create newInstance() static method in Fragment class;
* fi1 - /---/ create with one arguments
* fi2 - /---/ create with two arguments
```java
    private static final String KEY_ID = "KEY.ID";

    private String mId;

    public static TestFragment newInstance(String id) {
        TestFragment fragment = new TestFragment();
        Bundle args = new Bundle();
        args.putString(KEY_ID, id);
        fragment.setArguments(args);
        return fragment;
    }

    @Override
    public void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        mId = getArguments().getString(KEY_ID);
        
    }
```
 

