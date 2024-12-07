# Uninstall-NodeJS_NPM

```javascript
#!/bin/bash

# Stop any running Node.js processes
sudo pkill node

# Remove Node.js and npm
sudo rm -rf /usr/local/node
sudo rm /usr/local/bin/node
sudo rm /usr/local/bin/npm

# Remove any remaining files
sudo rm -rf /usr/local/lib/node_modules
sudo rm -rf /usr/local/include/node

# Remove package configuration
sudo rm -rf /usr/local/etc/npmrc
sudo rm -rf /usr/local/etc/node

# Verify uninstallation
node -v
npm -v
```
