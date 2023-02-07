# Ionic Sign in with Google
Sample Project that uses @codetrix-studio/capacitor-google-auth to implement "Sign in with Google" into an Ionic Capacitor App.

### Troubleshooting
<details>
  <summary>java.lang.RuntimeException: Unable to start activity ComponentInfo{....MainActivity}: java.lang.NegativeArraySizeException: -1</summary>
  
**You probably missed to add the plugin configuration in capacitor.config.ts:**
```js
{
  plugins: {
    GoogleAuth: {
      scopes: ['profile', 'email'],
      serverClientId: 'xxxxxx-xxxxxxxxxxxxxxxxxx.apps.googleusercontent.com',
      forceCodeForRefreshToken: true
    }
  }
}
```
</details>
