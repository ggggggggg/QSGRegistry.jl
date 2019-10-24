# QSGRegistry.jl
A Julia registry for projects related to the QSG.


# Update procedure
I think it goes like this
```
# To install Registrator
using Pkg
Pkg.add(Pkg.PackageSpec(url="https://github.com/GunnarFarneback/Registrator.jl"))

# To add a package OR to update it when a new version appears in the Project.toml file
using Registrator
dev Package
# edit the package Project.toml to have a new version
# push package
using PackageName
register(PackageName, "~/.julia/registries/QSGRegistry")
run(`git -C ~/.julia/registries/QSGRegistry push`)
```
