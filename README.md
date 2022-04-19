# SplashSample

Important pointers:
- Add dependency - implementation 'androidx.core:core-splashscreen:xxx'
 - MainActivity(Launcher activity) - Add **installSplashScreen()** 
    ```
    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        installSplashScreen()
        setContentView(R.layout.activity_main)
    }
    ```
  - Add theme extending Theme.SplashScreen. Add **windowSplashScreenBackground**, **windowSplashScreenAnimatedIcon** and **postSplashScreenTheme**. postSplashScreenTheme is must, which will be application theme. 
  - Menifest change - add this new theme. 
