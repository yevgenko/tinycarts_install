# Tinycarts_Install module

This module intended to temporary fix [issue #6145][1] in [magento][2] - ecommerce platform

## Installation

1. **Retrieve source code**

    Download repository as archive and extract into `app/code/local/Tinycarts/Install` dir.

    OR

    `git clone git://github.com/yviktorov/tinycarts_install.git app/code/local/Tinycarts/Install`

    OR

    `git submodule add git://github.com/yviktorov/tinycarts_install.git app/code/local/Tinycarts/Install`

    `git commit -m "add Tinycarts_Install module"`


2. **Enable module**

    Add `app/etc/modules/Tinycarts_Install.xml` into your project

    <?xml version="1.0"?>
    <config>
         <modules>
            <Tinycarts_Install>
                <active>true</active>
                <codePool>local</codePool>
            </Tinycarts_Install>
         </modules>
    </config>

3. **Clear cache**

    `rm -rf var/*` or via administration panel.

[1]: http://www.magentocommerce.com/bug-tracking/issue?issue=6145
[2]: http://www.magentocommerce.com/
