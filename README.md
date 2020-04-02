# File Path TH

We sometimes load config files from TemplateHaskell, e.g. `$(embedFile "./config/file")`. Unfortunately `stack build`
and `stack ghci` use different working directories, so this local path should sometimes be `./foo/bar/config/file`
instead. This package has utilities for embedding relative filepaths using Template Haskell.

From https://gist.github.com/jfischoff/7ee09a7c30e61d6b93cac1baa7f833cf
