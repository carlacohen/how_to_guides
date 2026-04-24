How to put an R chunk in the jupyter notebook

```
# use this chunk to set up being able to work with R
import logging

import rpy2.rinterface_lib.callbacks as rcb
import rpy2.robjects as ro
from rpy2.robjects import pandas2ri

rcb.logger.setLevel(logging.ERROR)


%load_ext rpy2.ipython
```

Then start the R chunk with: ```%%R```

You need to have R-cbrg listed in the text file here: ```~/jupyter/ccb.modules```

