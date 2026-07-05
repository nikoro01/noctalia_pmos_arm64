# noctalia_pmos_arm64
Noctalia Shell V5 for arm64 devices running postmarketOS

Tested and **built** on Wileyfox Swift 


<img width="720" height="1280" alt="image" src="https://github.com/user-attachments/assets/d9ae90c7-7953-4b85-9280-4ce2a0510463" /> <img width="720" height="1280" alt="image" src="https://github.com/user-attachments/assets/987dcd68-9bc0-49d7-beac-e27242214113" />



# Install dependencies
sudo apk add build-base meson ninja pkgconf git just

sudo apk add \
  wayland-dev wayland-protocols \
  mesa-dev \
  freetype-dev fontconfig-dev \
  cairo-dev pango-dev harfbuzz-dev \
  libxkbcommon-dev glib-dev \
  sdbus-cpp-dev pipewire-dev \
  linux-pam-dev polkit-dev \
  curl-dev libwebp-dev librsvg-dev \
  libqalculate-dev libxml2-dev \
  jemalloc-dev

# Create a directory for the build
mkdir -p ~/noctalia-arm64

# Extract the archive
tar -xzf noctalia-arm64-pmos.tar.gz -C ~/noctalia-arm64

# Go to the extracted folder
cd ~/noctalia-arm64

# Make sure it's executable
chmod +x noctalia

# Run it
./noctalia

