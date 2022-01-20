# Log out

Now that users can sign in, they'll need a way to sign out.

Open `'routes/auth.js'` and add this route at line 45, below the
`'/login/password'` route:

```js
router.post('/logout', function(req, res, next) {
  req.logout();
  res.redirect('/');
});
```

Return to the app, where you should be signed in, and click "Sign out."

We've now got a working app where users can sign in and sign out!  Next we
will let new users [sign up](../signup/).