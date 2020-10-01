<p align="center">
  <img src="https://i.imgur.com/LtUGnF3.png" width=500 />
</p>

<div align="center">
  <a href="https://github.com/sundowndev/PhoneInfoga/actions">
    <img src="https://img.shields.io/endpoint.svg?url=https://actions-badge.atrox.dev/sundowndev/PhoneInfoga/badge?ref=master" alt="build status" />
  </a>
  <a href="https://goreportcard.com/report/github.com/sundowndev/PhoneInfoga">
    <img src="https://goreportcard.com/badge/github.com/sundowndev/PhoneInfoga" alt="go report" />
  </a>
  <a href="https://codeclimate.com/github/sundowndev/PhoneInfoga/maintainability">
    <img src="https://api.codeclimate.com/v1/badges/3259feb1c68df1cd4f71/maintainability" />
  </a>
  <a href="https://codecov.io/gh/sundowndev/PhoneInfoga">
    <img src="https://codecov.io/gh/sundowndev/PhoneInfoga/branch/master/graph/badge.svg" />
  </a>
  <a href="https://github.com/sundowndev/PhoneInfoga/releases">
    <img src="https://img.shields.io/github/release/SundownDEV/PhoneInfoga.svg" alt="Latest version" />
  </a>
</div>

<h4 align="center">Advanced information gathering & OSINT framework for phone numbers</h4>

<p align="center">
  <a href="https://sundowndev.github.io/PhoneInfoga/">Documentation</a> •
  <a href="https://redocly.github.io/redoc/?url=https://raw.githubusercontent.com/sundowndev/PhoneInfoga/master/api/openapi.yml">API documentation</a> •
  <a href="https://demo.phoneinfoga.crvx.fr/">Demo instance</a> •
  <a href="https://medium.com/@SundownDEV/phone-number-scanning-osint-recon-tool-6ad8f0cac27b">Related blog post</a>
</p>

![](./docs/images/screenshot.png)

## About

PhoneInfoga is one of the most advanced tools to scan international phone numbers using only free resources. The goal is to first gather standard information such as country, area, carrier and line type on any international phone numbers with a very good accuracy. Then search for footprints on search engines to try to find the VoIP provider or identify the owner.

here is the one of the most used ohsint tools to track international phone number.

## Current status

**This project is under active development but is stable and production-ready. Numverify scan is pointless on demo instance because my server's IP got blocked due to spam**. [Roadmap is here](https://github.com/sundowndev/PhoneInfoga/projects/1).

This project has recently been rewritten in Go language (previously Python). Why ? To improve code base, maintainability, have a stronger test suite and be able to compile code base. PhoneInfoga v2 brings new features such as serving a REST API and a web client. Usage of scanners was improved in order to drop usage of Selenium/Geckodriver which has cause many users to have troubleshoots using the tool. You can still use the legacy version in [tag v1.11](https://github.com/sundowndev/PhoneInfoga/tree/v1.11) and the legacy Docker image (`sundowndev/phoneinfoga:legacy`). Some features were not included in the v2 MVP such as input/output CLI options. The roadmap of the project changed so we can focus on the web client features such as downloading scan results as CSV, Instagram/Whatsapp lookup, and more. **Version 2 does not scan Google results anymore**, [read more](https://sundowndev.github.io/PhoneInfoga/usage/#available-scanners).

## Features

- Check if phone number exists and is possible
- Gather standard informations such as country, line type and carrier
- OSINT footprinting using external APIs, Google Hacking, phone books & search engines
- Check for reputation reports, social media, disposable numbers and more
- Scan several numbers at once
- Use custom formatting for more effective OSINT reconnaissance
- **NEW**: Serve a web client along with a REST API to run scans from the browser
- **NEW**: Run your own web instance as a service
- **NEW**: Programmatic usage with Go modules

## Anti-features

- Does not claim to provide relevant or verified data, it's just a tool !
- Does not allow to "track" a phone or its owner in real time
- Does not allow to get the precise phone location
- Does not allow to hack a phone

![Footprinting process](https://i.imgur.com/qCkgzz8.png)

## License

[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fsundowndev%2FPhoneInfoga.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Fsundowndev%2FPhoneInfoga?ref=badge_shield)

This tool is licensed under the GNU General Public License v3.0.

[Icon](https://www.flaticon.com/free-icon/fingerprint-search-symbol-of-secret-service-investigation_48838) made by <a href="https://www.freepik.com/" title="Freepik">Freepik</a> from <a href="https://www.flaticon.com/" title="Flaticon">flaticon.com</a> is licensed by <a href="http://creativecommons.org/licenses/by/3.0/" title="Creative Commons BY 3.0" target="_blank">CC 3.0 BY</a>.

## Support

[![](docs/jetbrains.svg)](https://www.jetbrains.com/?from=sundowndev)

Thanks to [JetBrains](https://www.jetbrains.com/?from=sundowndev) for supporting my open-source projects.
