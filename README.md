# Obsidian function plot
Allows you to render 2d graphs inside a `function-plot` codeblock using the npm package `function-plot`

## function-plot codeblock

The function-plot codeblock uses YAML to specify its configuration.\
\
Functions are stored in the `data` object, X-axis data is stored in the xAxis object, same for Y-axis.\
\
For example:

````md
```function-plot
data:
	- fn: 2x
	- fn: x
	  closed: true
	- points:
		- [0,0.5]
		- [0.5,0]
	  fnType: points
	  graphType: polyline
xAxis:
	domain:
		- -1
		- 1
yAxis:
	domain:
		- -1
		- 1
```
````

Would produce the following graph:\
<img width="417" alt="image" src="https://github.com/tnichols217/obsidian-function-plot/assets/62992267/577982c3-6713-436e-9c2f-3e94a409c831">

## Reference guide

The entire reference guide for the specifications to the graph can be found [here](https://mauriciopoppe.github.io/function-plot/docs/interfaces/FunctionPlotOptions.html)\
Other examples for function-plot can be found [here](https://mauriciopoppe.github.io/function-plot/)

## Thanks

Huge thanks to [function-plot](https://www.npmjs.com/package/function-plot) by [Mauricio Poppe](https://github.com/mauriciopoppe)

---

### If you enjoy my plugin, please consider supporting me:

<a href="https://www.buymeacoffee.com/tnichols217" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" width="217" height="60" /></a>
[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/D1D0DF7HF)
