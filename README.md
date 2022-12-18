# SM-dyn-idletime
dynamically scales the maximum amount of time a client can be idle in a Source server based on the number of clients in that server

## V read this V
```
        "sm_dyn_idletime_ratio"
        dyn_idletime scales mp_idlemaxtime by (maxclients / currentplayers) * this ratio. This means that as players go up, mp_idlemaxtime goes down.
        Negative values scale with currentplayers directly, ignoring maxclients, meaning that as players go up, mp_idlemaxtime goes up.
        This value can't be zero.

        "sm_dyn_idletime_mintime",
        "Minimum amount (in minutes) that dyn_idletime will set mp_idlemaxtime to.

        "sm_dyn_idletime_maxtime",
        "Maximum amount (in minutes) that dyn_idletime will set mp_idlemaxtime to.
```
