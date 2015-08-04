# cookies-dialog

An Android library that displays to the user a dialog with the "cookies" message which is required by the EU laws.

# Include in your project

## How to use

This is a quick example of using this library in an application.
```java
public class MainActivity extends Activity {
  private CookieManager mCookieManager = new CookieManager(this);
  
  @Override
  protected void onCreate(Bundle savedInstanceState) {
    // your code here
    mCookieManager.showOnce(false); // Or pass "true" to show the dialog only to EU users
  }
  
  @Override
  protected void onDestroy() {
    // your code here
    mCookieManager.cancel();
  }
}
```

This will show the dialog only **once**. The next time the user opens the app the dialog will not be displayed.

# Developed by

Miguel Botón (Lowlevel Studios) - mboton@lowlevel-studios.com

# License

Copyright 2015 Miguel Botón

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
