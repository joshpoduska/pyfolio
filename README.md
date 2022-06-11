# Pyfolio from Quantopian

[pyfolio](https://github.com/quantopian/pyfolio) is a Python library for performance and risk analysis of financial portfolios developed by [Quantopian Inc](https://www.quantopian.com/). It works well with the [Zipline](https://github.com/quantopian/zipline) open source backtesting library. It can generate nice charts like this:

![strategy](raw/latest/img/drawdown-example.png?inline=true)

----

This project has sample notebooks you can launch and play with yourself.
After you've taken a look, if you want to run it yourself, click launch on the tool bar in the upper right corner:
![domino header](https://app.dominodatalab.com/domino/prudential/raw/e1aa3cadacf32c3a198f003c632e49ffc03ac05e/images/launch_button.png?inline=true)

Try it with the following notebooks:
- **Introduction**: You can get an overview of Pyfolio and the motivation behind it in [overview_slides.ipynb](/domino/pyfolio/view/overview_slides.ipynb)
- **Basic pyfolio examples**: [single_stock_example.ipynb](/domino/pyfolio/view/single_stock_example.ipynb) gives a simple example of using pyfolio to generate comprehensive visualizations about performance of one stock, and [sector_mapping_example.ipynb](/domino/pyfolio/view/sector_mapping_example.ipynb)  shows a more complex example, sector allocation plots in the positions tearsheet and PnL by sector in the round trips tearsheet.
- **Zipline example**: [zipline_algo_example.ipynb](/domino/pyfolio/view/zipline_algo_example.ipynb) shows how to use zipline to backtest a strategy (and then use pyfolio to visualize the results)


## Backtesting and comparing multiple strategies

In addition to hosting notebooks, Domino lets you run batch scripts, and it will keep your results tracked automatically. We've taken some of the zipline and pyfolio code and created a script that runs a backtest given a certain parameter. You can see examples of experiments we've run [here](https://app.dominodatalab.com/domino/pyfolio/results/56d292e72bf48768752a5f7c) and [here](https://app.dominodatalab.com/domino/pyfolio/results/56d292362bf48768752a5f75).

Because Domino tracks each experiment you run, you can compare results easily. In the example below, we use zipline to run a backtest, and we use pyfolio to generate visualizations of the performance of the strategy. Domino keeps the visualizations tracked, and lets us compare them so we can see which strategy performed better.

![compare1](raw/latest/img/compare-select.png?inline=true)

![compare2](raw/latest/img/compare-results.png?inline=true)

---

You can even choose to overlay the two visual results, to more easily see the differences:

![compare2](raw/latest/img/compare-overlay.png?inline=true)