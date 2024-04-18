# Homepage for the Camera Traps, AI and Ecology Workshop 2024

[Jenkyll Website](https://jekyllrb.com/) for the workshop, online at [camtraps2024.fh-ooe.at](camtraps2024.fh-ooe.at) and at [https://camtrap2024.github.io/](https://camtrap2024.github.io/). The repository is directly published online by GitHub-Pages. Content is stored file-based: mostly Markdown (.md) and YML (.yml) files.

**❗💥 Warning: Any changes you make in the main repository will be directly online! 💥❗**

## Open Points | Discussions | ToDos

- [x] Change LOGO and backround image
- [ ] Update Call
- [ ] Update Program
- [ ] Update Submission
- [ ] Proofreading and Removing Anything PPSN related
- [x] Update Front Page
- [x] Update Imprint
- [ ] Update About -> add Workshop Organizers (Paul, ...)
- [ ] Remove Google Analytics

# Local Development

If you want to make considerable changes to the website please test them first with a local setup.

These are the complete instructions for a development machine running under Microsoft Windows. The instructions should be very similar for any other operating system and have been verified on [Google Colab](https://colab.research.google.com/github/DigitalMediaLab-AT/digitalmedialab.at/blob/main/test_setup_GoogleColab.ipynb) (see [test_setup_GoogleColab](test_setup_GoogleColab.ipynb)).

### Install Git and Clone the Repository

Get the Git binaries from [https://git-scm.com/](https://git-scm.com/) or download GitHub Desktop from [https://desktop.github.com/](https://desktop.github.com/), then clone the repository to your local machine (e.g., `C:\Users\[User]\Documents\GitHub\digitalmedialab.at`).

### Install Ruby

Go to [http://rubyinstaller.org/](http://rubyinstaller.org/), download the latest installer for Ruby (Ruby+Devkit) and run it.

### Install Bundler and Jekyll

Once Ruby is installed, install Jekyll and its necessary plugins using [Bundler](https://bundler.io/). First, install the Bundler gem: `gem install jekyll bundler`. Then install the gems listed in the Gemfile by calling `bundle install`. For the later command you need have the repo in the current working path.

For further details, see [https://jekyllrb.com/docs/installation/](https://jekyllrb.com/docs/installation/).

### Start the Build System

The build workflow then uses bundle and can be started with: `bundle exec jekyll serve`.
A local server should be running at the address http://127.0.0.1:4000 and can be used to preview the website. Any changes and additions to markdown files should be imediatly visible. Note that changes to `_config.yml` need a restart of the build system!

# Acknowledgements and License

This website is based on the [PPSN website](https://ppsn2024.fh-ooe.at/) designed, developed and maintained by Jan Zenisek and Christian Haider. Thanks for the great work and the permission to use their code as a starting point for this website! The PPSN code is available at [https://github.com/ppsn2024/ppsn2024.github.io](https://github.com/ppsn2024/ppsn2024.github.io).
