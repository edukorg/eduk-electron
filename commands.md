flatpak-builder build br.com.eduk.app.yml --install --force-clean --user
flatpak build-bundle ~/.local/share/flatpak/repo eduk.flatpak br.com.eduk.app master

flatpak uninstall br.com.eduk.app
flatpak install '/home/Downloads/eduk-app-electron/flatpak/eduk.flatpak' --user
