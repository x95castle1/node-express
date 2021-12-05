# Accelerator Log

## Options
```json
{
  "includeK8s" : true,
  "projectDescription" : "",
  "projectName" : "node-express"
}
```
## Log
```
┏ engine (Chain)
┃  Info Running Chain(Combo, UniquePath)
┃ ┏ engine.transformations[0] (Combo)
┃ ┃  Info Combo running as Chain(Merge(merge), UniquePath(UseLast))
┃ ┃ engine.transformations[0].merge (Chain)
┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┏ engine.transformations[0].merge.transformations[0] (Merge)
┃ ┃ ┃  Info Running Merge(Combo, Combo, Combo, Combo, Combo)
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Exclude)
┃ ┃ ┃ ┃ engine.transformations[0].merge.transformations[0].sources[0].<combo> (Chain)
┃ ┃ ┃ ┃  Info Running Chain(Include, Exclude)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[0].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃  Info Will include [**]
┃ ┃ ┃ ┃ ┃ Debug .gitignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug LICENSE matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug README.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug k8s.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug kubernetes/deployment.yml matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug kubernetes/service.yml matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug kubernetes/skaffold.yml matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug package.json matched [**] -> included
┃ ┃ ┃ ┃ ┗ Debug server.js matched [**] -> included
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[0].<combo>.transformations[1] (Exclude)
┃ ┃ ┃ ┃ ┃  Info Will exclude [kubernetes/**, README.md, k8s.md, skaffold.md]
┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [kubernetes/**, README.md, k8s.md, skaffold.md] -> included
┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [kubernetes/**, README.md, k8s.md, skaffold.md] -> included
┃ ┃ ┃ ┃ ┃ Debug README.md matched [kubernetes/**, README.md, k8s.md, skaffold.md] -> excluded
┃ ┃ ┃ ┃ ┃ Debug k8s.md matched [kubernetes/**, README.md, k8s.md, skaffold.md] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/deployment.yml matched [kubernetes/**, README.md, k8s.md, skaffold.md] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/service.yml matched [kubernetes/**, README.md, k8s.md, skaffold.md] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/skaffold.yml matched [kubernetes/**, README.md, k8s.md, skaffold.md] -> excluded
┃ ┃ ┃ ┃ ┃ Debug package.json didn't match [kubernetes/**, README.md, k8s.md, skaffold.md] -> included
┃ ┃ ┃ ┗ ┗ Debug server.js didn't match [kubernetes/**, README.md, k8s.md, skaffold.md] -> included
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Chain(chain))
┃ ┃ ┃ ┃ engine.transformations[0].merge.transformations[0].sources[1].<combo> (Chain)
┃ ┃ ┃ ┃  Info Running Chain(Include, Chain)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[1].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃  Info Will include [package.json]
┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [package.json] -> excluded
┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [package.json] -> excluded
┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [package.json] -> excluded
┃ ┃ ┃ ┃ ┃ Debug k8s.md didn't match [package.json] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/deployment.yml didn't match [package.json] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/service.yml didn't match [package.json] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/skaffold.yml didn't match [package.json] -> excluded
┃ ┃ ┃ ┃ ┃ Debug package.json matched [package.json] -> included
┃ ┃ ┃ ┃ ┗ Debug server.js didn't match [package.json] -> excluded
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[1].<combo>.transformations[1] (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(ReplaceText)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[1].<combo>.transformations[1].transformations[0] (ReplaceText)
┃ ┃ ┃ ┗ ┗ ┗  Info Will replace [accelerator-description->, node-express->node-express]
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[2] (Combo)
┃ ┃ ┃ ┃  Info Condition (#includeK8s) evaluated to true
┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Chain(chain))
┃ ┃ ┃ ┃ engine.transformations[0].merge.transformations[0].sources[2].<combo> (Chain)
┃ ┃ ┃ ┃  Info Condition (#includeK8s) evaluated to true
┃ ┃ ┃ ┃  Info Running Chain(Include, Chain)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[2].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃  Info Will include [kubernetes/deployment.yml, kubernetes/service.yml]
┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [kubernetes/deployment.yml, kubernetes/service.yml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [kubernetes/deployment.yml, kubernetes/service.yml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [kubernetes/deployment.yml, kubernetes/service.yml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug k8s.md didn't match [kubernetes/deployment.yml, kubernetes/service.yml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/deployment.yml matched [kubernetes/deployment.yml, kubernetes/service.yml] -> included
┃ ┃ ┃ ┃ ┃ Debug kubernetes/service.yml matched [kubernetes/deployment.yml, kubernetes/service.yml] -> included
┃ ┃ ┃ ┃ ┃ Debug kubernetes/skaffold.yml didn't match [kubernetes/deployment.yml, kubernetes/service.yml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug package.json didn't match [kubernetes/deployment.yml, kubernetes/service.yml] -> excluded
┃ ┃ ┃ ┃ ┗ Debug server.js didn't match [kubernetes/deployment.yml, kubernetes/service.yml] -> excluded
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[2].<combo>.transformations[1] (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(ReplaceText)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[2].<combo>.transformations[1].transformations[0] (ReplaceText)
┃ ┃ ┃ ┗ ┗ ┗  Info Will replace [node-express->node-express]
┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[3] (Combo)
┃ ┃ ┃ ┃  Info Condition (#includeK8s) evaluated to true
┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Chain(chain))
┃ ┃ ┃ ┃ engine.transformations[0].merge.transformations[0].sources[3].<combo> (Chain)
┃ ┃ ┃ ┃  Info Condition (#includeK8s) evaluated to true
┃ ┃ ┃ ┃  Info Running Chain(Include, Chain)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[3].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃  Info Will include [kubernetes/skaffold.yml]
┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [kubernetes/skaffold.yml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [kubernetes/skaffold.yml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [kubernetes/skaffold.yml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug k8s.md didn't match [kubernetes/skaffold.yml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/deployment.yml didn't match [kubernetes/skaffold.yml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/service.yml didn't match [kubernetes/skaffold.yml] -> excluded
┃ ┃ ┃ ┃ ┃ Debug kubernetes/skaffold.yml matched [kubernetes/skaffold.yml] -> included
┃ ┃ ┃ ┃ ┃ Debug package.json didn't match [kubernetes/skaffold.yml] -> excluded
┃ ┃ ┃ ┃ ┗ Debug server.js didn't match [kubernetes/skaffold.yml] -> excluded
┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[3].<combo>.transformations[1] (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(ReplaceText, RewritePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[3].<combo>.transformations[1].transformations[0] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [node-express->node-express]
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].merge.transformations[0].sources[3].<combo>.transformations[1].transformations[1] (RewritePath)
┃ ┃ ┃ ┗ ┗ ┗ Debug Path 'kubernetes/skaffold.yml' matched '^(?<folder>.*/)?(?<filename>([^/]+?|)(?=(?<ext>\.[^/.]*)?)$)' with groups {ext=.yml, folder=kubernetes/, filename=skaffold.yml, g0=kubernetes/skaffold.yml, g1=kubernetes/, g2=skaffold.yml, g3=skaffold.yml, g4=.yml} and was rewritten to 'skaffold.yml'
┃ ┃ ┃ ┏ README (Combo)
┃ ┃ ┃ ┃  Info Combo running as Chain(Merge(merge), UniquePath(Append))
┃ ┃ ┃ ┃ README.merge (Chain)
┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┏ README.merge.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃  Info Running Merge(Combo, Combo)
┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Chain(chain))
┃ ┃ ┃ ┃ ┃ ┃ README.merge.transformations[0].sources[0].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[0].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [README.md]
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug k8s.md didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/deployment.yml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/service.yml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/skaffold.yml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug package.json didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug server.js didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[0].<combo>.transformations[1] (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[0].<combo>.transformations[1].transformations[0] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗ ┗ ┗  Info Will replace [node-express->node-express]
┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#includeK8s) evaluated to true
┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain(Include, Chain(chain))
┃ ┃ ┃ ┃ ┃ ┃ README.merge.transformations[0].sources[1].<combo> (Chain)
┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#includeK8s) evaluated to true
┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[1].<combo>.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [k8s.md]
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [k8s.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [k8s.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [k8s.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug k8s.md matched [k8s.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/deployment.yml didn't match [k8s.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/service.yml didn't match [k8s.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/skaffold.yml didn't match [k8s.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug package.json didn't match [k8s.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug server.js didn't match [k8s.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[1].<combo>.transformations[1] (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(ReplaceText, RewritePath)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[1].<combo>.transformations[1].transformations[0] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [node-express->node-express]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ README.merge.transformations[0].sources[1].<combo>.transformations[1].transformations[1] (RewritePath)
┃ ┃ ┃ ┃ ┗ ┗ ┗ ┗ Debug Path 'k8s.md' matched '^(?<folder>.*/)?(?<filename>([^/]+?|)(?=(?<ext>\.[^/.]*)?)$)' with groups {ext=.md, folder=null, filename=k8s.md, g0=k8s.md, g1=null, g2=k8s.md, g3=k8s.md, g4=.md} and was rewritten to 'README.md'
┃ ┃ ┃ ┃ ┏ README.merge.transformations[1] (UniquePath)
┃ ┃ ┗ ┗ ┗ Debug Multiple representations for path 'README.md', will concatenate them together
┃ ┃ ┏ engine.transformations[0].merge.transformations[1] (UniquePath)
┃ ┗ ┗ Debug Multiple representations for path 'package.json', will use the one appearing last 
┗ ╺ engine.transformations[1] (UniquePath)
```
