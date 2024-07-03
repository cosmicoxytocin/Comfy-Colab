Usage Guide
===

### Note: This notebook was built using Colab Pro. I'm unsure if Google still blocks ComfyUI for free-tier users.

---

### Steps
1. In the toolbar select: `Runtime -> Change runtime type -> {x} GPU` Where `x` is the GPU name.
    * I recommend `L4` for SDXL and SD3. (Pro Only)
    * For SD1.5, `T4` with `High-Ram` enabled.
2. Run `Connect Google Drive` Cell. A popup will ask you to sign into your Google account.
3. Run `Install/Update Comfy`.
    * Running this cell for the first time will install a new folder in your Google Drive.
        * The folder path is `MyDrive/Comfy/ComfyUI`
    * Running this cell after ComfyUI is installed will attempt to update ComfyUI to the latest master branch.
4. **Do Not** Run the `Download Model` cell. As of now, it is not finished. See [Install Guide](https://github.com/cosmicoxytocin/Comfy-Colab/blob/main/docs/install_models_sd3.md)
5. Run `Requirements` Cell. This will install the requirements to run ComfyUI in Google Colab.
6. Run `Launch ComfyUI` Cell. This cell will provide you with a cloudflare link for the interface. Before clicking the link, wait until you see the following cell output:

![Comfy-Wait](https://raw.githubusercontent.com/cosmicoxytocin/Comfy-Colab/main/assets/comfyColab_waitFor.png)
