# How to Contribute

The ITP/IMA Community Commitments is a community driven project. This repo is part of our effort to maintain a reachable and participative process in order to easily evolve the document and encourage contributions.

The Community Commitments follows the All-contributors specifications, which means that the community can get involved in any kind of support: like participation in discussions, co-authoring the document, as well as the website. We encourage any type of contribution, any change that helps the community grow a Best content and environment for all community members.

## Contributing Workflow

The basic flow for this participation is through the ITP/IMA Community Commitments Github. You can contribute by giving suggestions, or changing content with markdown. This allows us to change text, edit content without going deeper in the code.

To contribute through this repository, you must have a Github account.

Contributions are accessible through buttons like “Propose a Change”. The “Give Feedback” button can be found on the Get Involved page and other parts of the document. These two buttons will direct you to the github source, where you open a “pull request” to propose the changes, or give feedback by “reporting an issue”.

### Contributing with new/additional content, or updates

Using plain text editor Markdown, you can contribute to the Community Commitments.

**No code required!**

**Instructions to contribute changes to the Community Commitments document**

1. Go to the .md file where you want to make a change.
2. Press the edit button to edit the file.
3. Make changes to text.
4. Add a title and a description of the changes you made.
5. Title new branch
6. Commit changes

### Contributing from [Issues](https://github.com/ITPNYU/ITP-IMA-Community-Guidelines/issues)

To give feedback, or see what issues are pending, you can go to [Issues](https://github.com/ITPNYU/ITP-IMA-Community-Guidelines/issues) in this repository.

**Give a Feedback**
Before filing an issue, we encourage you to take a look at the list of issues. It might be addressed already.

**Work on New Issues**
If you want to contribute by working on an issue, you can check the issues list to see what hasn't been addressed.

**Website Development**
The website is built in Jekyll. You can contribute to the website using html, css, javascript or markdown. To contribute to developing the website or implementing design features, you can follow the Getting Started section in this document.

## Getting Started

If you want to help develop the ITP/IMA Community Commitments, here are the steps to get started:

### Setup

To run the website locally (on your computer) you’ll need to install jekyll on your computer. We recommend visiting Quickstart on the Jekyll documentation site to have a better understanding of the process.

**Prerequisites for running Jekyll locally:**

- Ruby version 2.4.0 or higher
- RubyGems
- GCC and Make

**To check which version you have:**

Ruby version
`ruby -v`

Gems version
`gem -v`

GCC and Make versions
`gcc -v`, `g++ -v`, and `make -v`

### Install Jekyll

1. Confirm that All prerequisites are installed
2. Install the jekyll and bundler gems:
   `gem install jekyll bundler`

### Developing in Jekyll

To make a local copy of this repository:

```
git clone https://github.com/ITPNYU/ITP-IMA-Code-of-Conduct.git
```

### Website structure

**Html files**

We use layouts to structure the website. Html files to structure the _.md_ documents, which are inside the _\_layouts_ folder. Each page is wrapped by a html.file named _header-footer.html_ Inside each html file there is a `{{ content }}` where you can reference other html and markdown files.

The html file has a reserved section on the top to reference another wrapper html file if needed.

Example:

```
---
layout: header-footer
---
```

**Markdown (.md) files**

Each markdown has a front matter section with a permalink variable that shows the path to the html.

To know more about Front Matter visit this [link](https://jekyllrb.com/docs/front-matter/).

There are two ways that we use to reference text between the html file and markdown:

1. _Liquid_ lets you modify any text link inside html elements, like buttons. Inside the html file, the objects tell Liquid where to show content on a page.

Input in html file
`{{ page.my_title }}`

The _markdown_ references that variable from the Front Matter section:

```
---
my_title: “This is the Title”
---
```

2. To manage most of the content of the page, the website uses the liquid tag using two curly braces e.g. `{{ content }}` in the html file to insert content from the markdown.

In the markdown file the plain text reference.

Any content written in the markdown file is going to be reflected in the area that the tag `{{ content }}` has reserved.

### Running locally (on your computer)

**Run website**

To run locally for the first time:
`bundle exec jekyll serve`

After you’ve run it once, you can just use:
`jekyll serve`

## Additional Resources

- [Jekyll](https://jekyllrb.com/)
- [Liquid](https://shopify.github.io/liquid/basics/introduction/)
- [About Issues](https://docs.github.com/en/github/managing-your-work-on-github/about-issues)
- [Editing Files in Another Users Repository](https://docs.github.com/en/github/managing-files-in-a-repository/editing-files-in-another-users-repository)
- [Cloning a Repository](https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository)
