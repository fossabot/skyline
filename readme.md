## Skyline

version - Luminosity

![skyline web app](skyline.png)
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FVictorPronchev%2Fskyline.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2FVictorPronchev%2Fskyline?ref=badge_shield)

Skyline is a near real time anomaly detection system, built to enable
passive monitoring of hundreds of thousands of metrics, without the need
to configure a model/thresholds for each one, as you might do with Nagios.
It is designed to be used wherever there are a large quantity of
high-resolution time series which need constant monitoring. Once a metrics
stream is set up (from StatsD or Graphite or another source), additional
metrics are automatically added to Skyline for analysis. Skyline's easily
extended algorithms attempt to automatically detect what it means for each
metric to be anomalous.

## Improvements to the original Etsy Skyline
 
- Improving the anomaly detection methodologies used in the 3-sigma context.
- Extending Skyline's 3-sigma methodology to enable the operator and Skyline to
  handle seasonality in metrics.
- The addition of an anomalies database for learning and root cause analysis.
- Adding the ability for the operator to train Skyline and have Skyline learn
  things that are NOT anomalous using a time series similarities comparison
  method based on features extraction and comparison using the tsfresh
  package.
- Adding the ability to Skyline to determine what other metrics are related to
  an anomaly event using cross correlation analysis of all the metrics using
  Linkedin's luminol library when an anomaly event is triggered and
  recording these in the database to assist in root cause analysis.

## Documentation

All the Skyline documentation is available online at
http://earthgecko-skyline.readthedocs.io/en/latest/

The documentation for your version is also viewable in a clone locally in your
browser at `file://<PATH_TO_YOUR_CLONE>/docs/_build/html/index.html` and via the
the Skyline Webapp frontend.

## Other

https://gitter.im/earthgecko-skyline/Lobby


## License
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FVictorPronchev%2Fskyline.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2FVictorPronchev%2Fskyline?ref=badge_large)