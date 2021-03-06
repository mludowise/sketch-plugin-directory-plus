# Sketch Plugin Directory Plus

Enhances the [Sketch Plugin Directory](https://github.com/sketchplugins/plugin-directory/) with additional metadata about each plugin.

The [plugins-metadata.json](https://github.com/mludowise/sketch-plugin-directory-plus/blob/master/plugins-metadata.json) and [log.md](https://github.com/mludowise/sketch-plugin-directory-plus/blob/master/log.md) files are generated every hour from the latest plugins in the [Sketch Plugin Directory](https://github.com/sketchplugins/plugin-directory/).

## Fields

**owner** &ndash; The GitHub owner of the repository. This is either a user or organization. *Note that for plugins that do not have a GitHub repository, this may not correspond to a valid GitHub owner.*

**name** (nullable) &ndash; The GitHub repository name. *Note that for plugins that do not have a GitHub repository, this may not correspond to a valid GitHub repository and may be nil.*

**author** &ndash; The display name for the author of this repository. Defaults to **owner** if none is provided.

**title** &ndash; The display name for the plugin. Defaults to **name** if none is provided.

**homepage** (nullable) &ndash; A URL pointing to the homepage for this plugin. If none is provided and this plugin corresponds to a valid GitHub repository, this will default to the homepage set in GitHub. If no homepage is set in GitHub, this will default to the GitHub repository URL.

**description** &ndash; A human-readable description of what this plugin does.

**added** &ndash; The date this plugin was added to the [Plugin Directory](https://github.com/sketchplugins/plugin-directory/). This may correspond to the time the plugin was detected (within 1 hour) and not the precise time it was added.

**icon** (nullable) &ndash; A URL for a PNG icon for this plugin. Currently, the only way to specify an icon for a plugin is to put it in the path **[plugin name].sketchplugin/Contents/Resources/icon.png** location in the GitHub project for a plugin.

**gh_url** (nullable) &ndash; The URL for the GitHub repository corresponding to this plugin, if it exits (based on the **owner** and **name**).

**gh_branch** (nullable) &ndash; The default branch for the GitHub repository corresponding to this plugin, if it exists.

**gh_updated** (nullable) &ndash; The date this repository was updated in GitHub, if it exists. This date corresponds to the the last commit date for the default repository branch if it exists, otherwise it corresponds to the **pushed_at** date of the repository.

**gh_stars** (nullable) &ndash; The number of stargazers for this repository on GitHub, if it exists.

**gh_issues** (nullable) &ndash; The number of open issues for this repository on GitHub, if it exists.

**man_identifier** (nullable) &ndash; The **identifier** field from the manifest.json file of the plugin.

**man_version** (nullable) &ndash; The **version** field from the manifest.json file of the plugin.

**man_compatible_version** (nullable) &ndash; The **compatibleVersion** field from the manifest.json file of the plugin.

## Log.md

Problems found during the last time the [plugins-metadata.json](https://github.com/mludowise/sketch-plugin-directory-plus/blob/master/plugins-metadata.json) file was generated can be found in [log.md](https://github.com/mludowise/sketch-plugin-directory-plus/blob/master/log.md).

## Contribution

To add a plugin to this directory, follow the contribution instructions for the official [Plugin Directory](https://github.com/sketchplugins/plugin-directory/). This directory will be automatically updated within an hour after the changes have been committed.

To request any additional information to this project, make a request by filing an [Issue](https://github.com/mludowise/sketch-plugin-directory-plus/issues).
