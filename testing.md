# Testing

## Types of testing

### Unit tests
Unit tests are the first line of defense for any new regressions in the build. A unit test validates the smallest pieces of an application and runs in complete isolation of the rest of the app and the app’s environment.
Unit tests are great at testing individual components of a system, but unfortunately many bugs arise when all the moving parts come together. This is another reason they function best as a first step, a pre-cursor to integration tests.

### Integration tests
Integration tests extend test coverage by exercising the system’s API. Instead of developer provided data, integration tests have data sent to an endpoint and manipulated by the same services that users will be taking advantage of in production.
- Quick way to test system services.
- Can run without a user.
- Validate system processes with great speed.
- Tests are reliable.

These tests produce little false positive results and if a test fails it provides the testers with good debugging info.

### UI tests
UI tests provide end-to-end coverage and make sure that system is stable and satisfies critical business requirements by interacting with the user interface. UI tests are ideal tests to be written by a QA team because they don’t require any knowledge of the code base. Test runs in the same way that a user would so QA can automate their favorite test cases. Test Engineers love these tests for a couple of reasons:

- Stable builds are guaranteed before it gets into a tester’s hands.
- Compatibility: the same test can be run on different devices to ensure that your app works on any OS/Device combination.

### Patterns

#### Testing pyramid

![Testing pyramid](https://raw.githubusercontent.com/ricardocasares/grow/assets/automation-pyramid-1.png "Testing pyramid")

#### Ice cone anti-pattern
![Ice cone anti-pattern](https://raw.githubusercontent.com/ricardocasares/grow/assets/automation-pyramid-ice-cream.png "Ice cone anti-pattern")
