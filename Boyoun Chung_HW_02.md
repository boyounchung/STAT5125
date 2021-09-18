```julia
#Problem 1

x = Vector(1:100)
y = x.^2
a = sum(y)
b = (sum(x)).^2
b - a
```




    25164150




```julia
using CSV
using DataFrames
CSV.File("triangle.csv")
triangle = DataFrame(CSV.File("triangle.csv"))

```




<div class="data-frame"><p>0 rows × 1 columns</p><table class="data-frame"><thead><tr><th></th><th>triangle.csv</th></tr><tr><th></th><th title="Missing">Missing</th></tr></thead><tbody></tbody></table></div>




```julia
for(i in 1:nrow(triangles)){
    if (triangles$a[i] + triangles$b[i] > triangles$c[i]
        & triangles$a[i] + triangles$c[i] > triangles$b[i] &
        triangles$c[i] + triangles$b[i] > triangles$a[i]){
        triangles$isTriangle[i] = 1
        }else{
        triangle$isTriangle[i] = 0
        }
    }
```


    syntax: unexpected "}"

    

    Stacktrace:

     [1] top-level scope

       @ In[47]:9

     [2] eval

       @ ./boot.jl:360 [inlined]

     [3] include_string(mapexpr::typeof(REPL.softscope), mod::Module, code::String, filename::String)

       @ Base ./loading.jl:1116

