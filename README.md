# Battery Trading Benchmark

## What is it?

**Battery Trading Benchmark** is an open source tool to determine the optimal value an Energy Storage System (ESS) can earn on a specific electricity market.
It aims to be the market standard in evaluating an ESS system on different energy markets.
This tool should become a powerful, open source and intuitive manner to evaluate any kind of ESS on the electricity market.
This tool is maintained by [GIGA Storage][GIGA Home Page], a company that specialises in investing, realising and operating large-scale (Battery) Energy Storage Systems in The Netherlands and Europe.

## Running Battery Trading Benchmark

1. Create a virtual python environment and install packages

```console
pip install -r requirements.txt
```

2. Create your Streamlit secrets file (`.streamlit/secrets.toml`) using the `.streamlit/secrets.toml.example` file as a template

3. Run the Streamlit app locally

```console
streamlit run .\main.py
```

### Docker

It is also possible to run this tool using Docker.

1. Build the image

```console
docker build . -t battery-trading-benchmark
```

2. Run the image

```console
docker run -p 8501:8501 --env ENTSOE_API_KEY="place-uuid-here" -d battery-trading-benchmark
```

## License

See license file.

## Discussion and Development

Most development discussions take place on GitHub in this repository, via the GitHub issue tracker.

## Contributing

All contributions, bug reports, bug fixes, documentation improvements, enhancements and ideas are welcome.

A detailed overview on how to contribute can be found in the [contributing guide][GigaStorage Contributing Guide].

As contributers and maintainers to this project, you are expected to abide by the GigaStorage Code of Conduct.
More information can be found at: [Contributor Code of Conduct][GigaStorage Code of Conduct].

[GIGA Home Page]: https://giga-storage.com/en/
[GigaStorage Contributing Guide]: https://github.com/GigaStorage/.github/blob/main/CONTRIBUTING.md
[GigaStorage Code of Conduct]: https://github.com/GigaStorage/.github/blob/main/CODE_OF_CONDUCT.md
