<p align="center">
  <a href="https://mpds.f3m.pt/" rel="noopener" target="_blank"><img width="350" src="https://i.imgur.com/OANOfLI.png" alt="MPDS logo"></a></p>
</p>

<h1 align="center">MpDS Vertical-Nav</h1>

<div align="center">

[React](https://reactjs.org/) component for faster and simpler web development.

<!--
[![license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/mui-org/material-ui/blob/master/LICENSE)
[![npm latest package](https://img.shields.io/npm/v/@material-ui/core/latest.svg)](https://www.npmjs.com/package/@material-ui/core)
[![npm next package](https://img.shields.io/npm/v/@material-ui/core/next.svg)](https://www.npmjs.com/package/@material-ui/core)
[![npm downloads](https://img.shields.io/npm/dm/@material-ui/core.svg)](https://www.npmjs.com/package/@material-ui/core)
[![CircleCI](https://img.shields.io/circleci/project/github/mui-org/material-ui/next.svg)](https://app.circleci.com/pipelines/github/mui-org/material-ui?branch=next)
[![Coverage Status](https://img.shields.io/codecov/c/github/mui-org/material-ui/next.svg)](https://codecov.io/gh/mui-org/material-ui/branch/next)
[![Follow on Twitter](https://img.shields.io/twitter/follow/MaterialUI.svg?label=follow+Material-UI)](https://twitter.com/MaterialUI)
[![Dependabot Status](https://api.dependabot.com/badges/status?host=github&repo=mui-org/material-ui)](https://dependabot.com)
[![Average time to resolve an issue](https://isitmaintained.com/badge/resolution/mui-org/material-ui.svg)](https://isitmaintained.com/project/mui-org/material-ui 'Average time to resolve an issue')
[![Crowdin](https://badges.crowdin.net/material-ui-docs/localized.svg)](https://translate.material-ui.com/project/material-ui-docs)
[![Open Collective backers and sponsors](https://img.shields.io/opencollective/all/material-ui)](https://opencollective.com/material-ui) -->

</div>

## Installation

MpDS Vertical-Nav is available as an [npm package](npm i mpds-vertical-nav).

```sh
// with npm
npm i mpds-vertical-nav

```

## Usage

Here is a quick example to get you started, **it's all you need**:

```tsx
import * as React from "react";
import MpDSVerticalNav from "mpds-vertical-nav";

function App() {
  return <MpDSVerticalNav barExtended="true"></MpDSVerticalNav>;
}

ReactDOM.render(<App />, document.querySelector("#app"));
```

<h4>Props</h4>

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Description</th>
      <th>Default</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <span>sectionsItems</span>
      </td>
      <td>
        <div>
          <span>Array that has all the information about the section items: link, icon and itemTitle.</span>
        </div>
        <div>
          <div>
            <span>Array<{ link: string; icon: string; itemTitle: string }></span>
          </div>
        </div>
      </td>
      <td>
        <span>[
            {
              link: "/",
              icon: (
                <IconButton
                  color="primary"
                  size="small"
                  aria-label="f3m"
                  className="align-text-top">
                  <DashboardIcon fontSize="large"></DashboardIcon>
                </IconButton>
              ),
              itemTitle: (
                <Box
                  fontSize={14}
                  fontWeight={700}
                  fontFamily="Nunito"
                  style={{
                    paddingLeft: 10,
                    marginTop: "auto",
                    marginBottom: "auto",
                    textTransform: "uppercase",
                    color: "#3f51b5",
                    width: 170,
                    textAlign: "left",
                    height: 40,
                    lineHeight: 3,
                  }}>
                  Dashboard
                </Box>
              ),
            },
            {
              link: "/settings",
              icon: (
                <IconButton
                  color="primary"
                  size="small"
                  aria-label="f3m">
                  <SettingsIcon fontSize="large" />
                </IconButton>
              ),
              itemTitle: (
                <Box
                  fontSize={14}
                  fontWeight={700}
                  fontFamily="Nunito"
                  style={{
                    paddingLeft: 10,
                    marginTop: "auto",
                    marginBottom: "auto",
                    textTransform: "uppercase",
                    color: "#3f51b5",
                    width: 170,
                    textAlign: "left",
                    height: 40,
                    lineHeight: 3,
                  }}>
                  Settings
                </Box>
              ),
            },
            {
              link: "/wounds",
              icon: (
                <IconButton
                  color="primary"
                  size="small"
                  aria-label="f3m">
                  <HealingIcon fontSize="large"></HealingIcon>
                </IconButton>
              ),
              itemTitle: (
                <Box
                  fontSize={14}
                  fontWeight={700}
                  fontFamily="Nunito"
                  style={{
                    paddingLeft: 10,
                    marginTop: "auto",
                    marginBottom: "auto",
                    textTransform: "uppercase",
                    color: "#3f51b5",
                    width: 170,
                    textAlign: "left",
                    height: 40,
                    lineHeight: 3,
                  }}>
                  WOUNDS
                </Box>
              ),
            };
          ]</span>
      </td>
    </tr>
    <tr>
      <td>
        <span>barExtended</span>
      </td>
      <td>
        <div>
          <span>Boolean value of the bar extension state</span>
        </div>
        <div>
          <div>
            <span>boolean</span>
          </div>
        </div>
      </td>
      <td>
        <span>false</span>
      </td>
    </tr>
    <tr>
      <td>
        <span>selectedNavTabBackground</span>
      </td>
      <td>
        <div>
          <span>Background color of the selected nav.</span>
        </div>
        <div>
          <div>
            <span>string</span>
          </div>
        </div>
      </td>
      <td>
        <span>"#3f51b534"</span>
      </td>
    </tr>
    <tr>
      <td>
        <span>selectedNavTabBorderColor</span>
      </td>
      <td>
        <div>
          <span>Border color of the selected nav.</span>
        </div>
        <div>
          <div>
            <span>string</span>
          </div>
        </div>
      </td>
      <td>
        <span>"#3f51b5"</span>
      </td>
    </tr>
    <tr>
      <td>
        <span>onClickToogleIcon</span>
      </td>
      <td>
        <div>
          <span>onClick to toogle the menu.</span>
        </div>
        <div>
          <div>
            <span>React.MouseEventHandler<HTMLButtonElement></span>
          </div>
        </div>
      </td>
      <td>
        <span>"#3f51b5"</span>
      </td>
    </tr>
  </tbody>
</table>
<br>
Yes, it's really all you need to get started! Try it in:
[CodeSandbox](https://codesandbox.io/)
<br>

## License

No License. "(...) nobody else can copy, distribute, or modify your work without being at risk of take-downs, shake-downs, or litigation."
