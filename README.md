# LIVETemplate
Live Template for Android Studio

* cmvp - Check mvp view for null
```
if(getMvpView() != null){
    
}
```

* sa1 - Create new Intent in Activity class; 
* sa2 - /---/ create with two arguments
```
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
