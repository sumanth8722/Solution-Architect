
# Ref: https://www.terraform.io/cli/config/config-file

Put this in your ~/.terraformrc.
(by default this file does not exist, create this file .terraformrc add below cache key value. Keep the file locally anywhere and set the path by TF_CLI_CONFIG_FILE

plugin_cache_dir   = "$HOME/.terraform.d/plugin-cache"
disable_checkpoint = true

Then create the cache directory:
mkdir -p $HOME/.terraform.d/plugin-cache

export TF_PLUGIN_CACHE_DIR="$HOME/.terraform.d/plugin-cache"
