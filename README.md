# QSGRegistry.jl
A Julia registry for projects related to the QSG.


# Update procedure
I think it goes like this
```
using Pkg
Pkg.add(Pkg.PackageSpec(url="https://github.com/GunnarFarneback/Registrator.jl"))
using Registrator
dev Package
# edit the package Project.tml to have a new version
# push package
using PackageName
register(PackageName, "~/.julia/dev/QSGRegistry")
run(`git -C ~/.julia/dev/QSGRegistry push`)
```
