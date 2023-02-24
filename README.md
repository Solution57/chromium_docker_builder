** Chromium docker builder **


Usage:

Create .env file with the following content

```
CHROMIUM_BRANCH="110.0.5481.61"
GIT_SERVER="<GIT_SERVER>"
GIT_USER="builder"

CHROMIUM_URL="a/chromium/src"
HTTP_PASSWORD="<GIT_HTTP_PASSWORD>"

# Apply GN args
GN_ARGS="target_os=\"android\" target_cpu = \"arm64\"  is_debug = false proprietary_codecs = true  is_chrome_branded = false  is_component_build = false use_official_google_api_keys = false ffmpeg_branding = \"Chrome\" system_webview_package_name = \"com.google.android.webview\" use_openh264=true  enable_ffmpeg_video_decoders = true"

BUILD_TARGET=system_webview_apk
```
