# Grammar Selector package

See how the travis build works.

https://discuss.atom.io/t/load-developing-package/2554/5
has info about developing a package.

Javascript for console:

    atom.grammars.getGrammars().map(function(x) { return x.scopeName;})

  ["text.plain.null-grammar", "source.cpp", "source.coffee", "source.litcoffee", "source.c", "source.clojure", "source.css", "source.nant-build", "source.csx", "source.cs", "text.git-rebase", "source.git-config", "text.git-commit", "source.gfm", "text.html.gohtml", "text.html.basic", "source.go", "source.gotemplate", "text.hyperlink", "source.java-properties", "source.java", "text.junit-test-report", "text.html.jsp", "source.css.less", "source.js", "source.json", "source.js.regexp", "source.sql.mustache", "source.makefile", "text.html.mustache", "source.objcpp", "source.strings", "source.plist", "text.html.php", "source.perl", "source.objc", "text.xml.plist", "text.python.console", "text.python.traceback", "source.python", "text.html.erb", "source.regexp.python", "text.html.ruby", "source.ruby", "source.ruby.rails.rjs", "source.js.rails source.js.jquery", "source.sql.ruby", "source.ruby.rails", "source.sass", "source.css.scss", "text.shell-session", "source.sql", "source.shell", "text.plain", "text.todo", "text.xml.xsl", "source.yaml", "source.toml", "text.xml"]





This seems interesting perhaps:
https://atom.io/packages/editor-settings

See also http://editorconfig.org/

Here is the config.json with different settings for markdown and utilizing the
file-types editor:

    "*":
      editor:
        invisibles: {}
        fontSize: 12
        showInvisibles: true
        showIndentGuide: true
        softWrap: true
      core:
        themes: [
          "atom-light-ui"
          "atom-light-syntax"
        ]
      "file-types":
        "html.md.erb": "source.gfm"
      "exception-reporting":
        userId: "11cdcabc-89ad-ae1c-9de8-79966de5f7d9"
      welcome:
        showOnStartup: false
      "todo-show":
        ignoreThesePaths: [
          "app/vendor"
          "test/libs"
        ]
    ".gfm.source":
      editor:
        softWrap: true
