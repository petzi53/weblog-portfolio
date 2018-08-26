+++
# Hero Carousel widget.
widget = "hero_carousel"
active = true
date = 2017-10-15T00:00:00

# Order that this section will appear in.
weight = 1

# Slide interval.
# Use `false` to disable animation or enter a time in ms, e.g. `5000` (5s).
interval = 7000

# Minimum slide height.
# Specify a height to ensure a consistent height for each slide.
height = "300px"

# Slides.
# Duplicate an `[[item]]` block to add more slides.
[[item]]
  title = "What is ORCID? Why register?"
  content = "ORCID is a personal, digital, international and persistent name identifier. It is connecting research and researchers."
  align = "center"

  overlay_color = "#666"  # An HTML color value.
  overlay_img = "headers/wood-wide.jpg"
  overlay_filter = 0.1  # Darken the image. Value in range 0-1.
  
  cta_label = "Start reading"
  cta_url = "/2018/08/26/orcid-researchers-uniquely-identified/"
  cta_icon_pack = "fa"
  cta_icon = "book"
  
[[item]]
  title = "Using themes with blogdown"
  content = "How to choose a Hugo theme? How to start with a theme? Read the whole article or just the [resulting guidelines](/2018/07/19/blogdown-using-themes/#guidelines)."
  align = "center"  # Choose `center`, `left`, or `right`.

# Overlay a color or image (optional).
#   Deactivate an option by commenting out the line, prefixing it with `#`.
  overlay_color = "#666"  # An HTML color value.
  overlay_img = "headers/bubbles-wide.jpg"
  overlay_filter = 0.3  # Darken the image. Value in range 0-1.

# Call to action button (optional).
#   Activate the button by specifying a URL and button label below.
#   Deactivate by commenting out parameters, prefixing lines with `#`.

# use old (4.7 font-awesome icons: https://fontawesome.com/v4.7.0/icons/)

  cta_label = "Start reading full article"
  cta_url = "/2018/07/19/blogdown-using-themes/"
  cta_icon_pack = "fa"
  cta_icon = "book"


# [[item]]
#  title = "Right"
#  content = "I am right aligned :smile:"
#  align = "right"

#  overlay_color = "#333"  # An HTML color value.
#  overlay_img = ""  # Image path relative to your `static/img/` folder.
#  overlay_filter = 0.5  # Darken the image. Value in range 0-1.

+++
