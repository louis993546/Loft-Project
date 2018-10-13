# Client onboarding

## Flow

Psuedo code:

```
flow("onboarding") {
    node("start", startingPoint = true) {
        show("splash screen")
        wait(4000, and = { initFinished() }) {
            goto {
                if (firstTime) "onboarding"
                else "main"
            }
        }
    }
    node("onboarding") {
        show("what is loft")
        button("next") {
            goto { "onboarding2" }
        }
    }
    node("onboarding2") {
        show("what can loft do")
        button("next") {
            goto { "onboardingLast" }
        }
        button("back") {
            goto { "onboarding" }
        }
    }
    node("onboardingLast") {
        show("want to try?")
        button("make new loft") {
            goto { "makeNewLoft" }
        }
        button("join loft") {
            goto { "joinLoft" }
        }
    }
    node("makeNewLoft") {
        show("$formToFill")
        button("CREATE") {
            goto { 
                if (SUCCESS) "homeScreen"
                else "error"
            }
        }
    }
    node("joinLoft") {
        show("$signInForm")
        button("request") {
            goto { "requestToJoinPleaseWait" }
        }
    }
    node("requestToJoinPleaseWait") {
        show("We will let you know the moment when your roommate confirmed you just moved in (jazz hands emoji)")
    }
}
```

### Sign up (Make new loft)

- Form
    - Loft name
    - Your name

### Sign in (Join existing loft)

- User should not need to create account/sign in with their social account
- User has to enter a 9 character (essentially loft ID) to request to join
    - `0`-`9` and `.` (i.e. `numberPad` on iOS)
- Exsiting user then confirm/deny the request to join