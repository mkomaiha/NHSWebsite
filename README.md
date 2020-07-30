# NHSWebsite
## How to project setup

https://dev.to/brunolemos/tutorial-100-code-sharing-between-ios-android--web-using-react-native-web-andmonorepo-4pej

### Starting a new React Native project
`react-native init nhs`
`cd nhs`
`git init && git add . -A && git commit -m "Initial commit"`

### Turning our folder structure into a monorepo
- `cd {project_root}`
- `rm yarn.lock && rm -rf node_modules`
- `mkdir -p packages/components/src packages/mobile packages/web`
- Move all the files (except .git) to the packages/mobile folder
- Edit the name field on packages/mobile/package.json from nhs to mobile
- Create this package.json at the root directory to enable Yarn Workspaces:
- Create a .gitignore at the root directory
- `yarn`
