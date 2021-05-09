# Compatibility
The following illustration shows how various packages under the
Funcky umbrella are compatible with each other.

```
                                    ┌─────── Released ────────┐ ┌─ Planned ─┐
                                    ┊                         ┊ ┊           ┊
                                    ┌───────────┐ ┌───────────┐ ┌───────────┐
┌─── Funcky                         │    1.x    │ │    2.x    │ │    3.x    │
│                                   └───────────┘ └───────────┘ └───────────┘
│                                                 ┊             ┊           ┊
│                                                 ┊             ┌───────────┐
│ ┌─ (System.Linq.Async)                          ┊             │    5.x    │
│ │                                               ┊             └───────────┘
│ │                                               ┊             ┊           ┊
│ │                                               ┊             ┌───────────┐
├─┴─ Funcky.Async                                 ┊             │    1.x    │
│                                                 ┊             └───────────┘
│                                                 ┊             ┊           ┊
│                                                 ┌─────────────────────────┐
│ ┌─ (XUnit)                                      │           2.x           │
│ │                                               └─────────────────────────┘
│ │                                               ┊             ┊           ┊
│ │                                               ┌─────────────────────────┐
├─┴─ Funcky.XUnit                                 │         0.1.x           │
│                                                 └─────────────────────────┘
│                                                 ┊             ┊           ┊
│                                                 ┌───────────┐ ┌───────────┐
├─── Funcky.Money                                 │    1.x    │ │    2.x    │
│                                                 └───────────┘ └───────────┘
│                                                 ┊                         ┊
│                                                 ┌────────┐ ┌─────┐ ┌──────┐
│ ┌─ (Microsoft.EntityFrameworkCore)              │ >3.1.x │ │ 4.x │ │ 5.x  │
│ │                                               └────────┘ └─────┘ └──────┘
│ │                                               ┊                         ┊
│ │                                               ┌─────────────────────────┐
└─┴─ Funcky.EntityFrameworkCore                   │         0.1.x           │
                                                  └─────────────────────────┘
```

## Packages
### [Funcky](https://github.com/polyadic/funcky)
[![NuGet package](https://buildstats.info/nuget/Funcky)](https://www.nuget.org/packages/Funcky)

### [Funcky.Xunit](https://github.com/polyadic/funcky)
[![NuGet package](https://buildstats.info/nuget/Funcky.Xunit)](https://www.nuget.org/packages/Funcky.Xunit)

### [Funcky.Money](https://github.com/polyadic/funcky-money)
[![NuGet package](https://buildstats.info/nuget/Funcky.Money)](https://www.nuget.org/packages/Funcky.Money)

### [Funcky.EntityFrameworkCore](https://github.com/polyadic/funcky-efcore)
[![NuGet package](https://buildstats.info/nuget/Funcky.EntityFrameworkCore)](https://www.nuget.org/packages/Funcky.EntityFrameworkCore)

## Explanation
* Dependencies always point upwards.
* The `x` in a version stands for the newest released version.
* Dotted lines (`┊`) indicate the mayor releases from Funcky.
* Packages in parenthesis are important external dependencies.