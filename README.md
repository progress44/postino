<!-- PROJECT LOGO -->
<br />
<p align="center">

  <h1 align="center">POSTINO</h1>

  <p align="center">
    A new breath of life to wp_mail.
  </p>
</p>



<!-- TABLE OF CONTENTS -->
## Table of Contents

- [Table of Contents](#table-of-contents)
- [About The Project](#about-the-project)
  - [How it works](#how-it-works)
- [Getting Started](#getting-started)
  - [Updates](#updates)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)



<!-- ABOUT THE PROJECT -->
## About The Project
![Product Name Screen Shot][screenshot]
**Postino** was built to make sending emails via WP the easiest it can get. It provides a setting page where you can set the SMTP parameters, but, in case of batch installations, you can even put a configuration file in your theme. 
### How it works
Postino overrides the WordPress' core function `wp_mail()`, by adding custom options to use with SMTP. The SMTP sending is done via the [PHPMailer extension](https://code.google.com/a/apache-extras.org/p/phpmailer/), which you can substitute with any SMTP library you prefer.



<!-- GETTING STARTED -->
## Getting Started

You can just clone this repository inside your `wp-content/plugins` folder, or [download the installable zip](https://github.com/simmontali/postino/zipball/master) and install it via the WordPress dashboard. 

### Updates
Right now, Postino doesn't update itself via the WordPress updates. That is a WIP and will be implemented in the future.


<!-- USAGE EXAMPLES -->
## Usage

To use Postino, just install it and set up your SMTP server in the settings page. Don't want to do that? Just include a `postino.json` file in your active theme folder. Postino will look for it and load the settings in it. A `postino.json` file defines these settings:

```json
{
    "smtp_secure": "ssl",
    "smtp_port": 465,
    "smtp_server": "smtp.gmail.com",
    "smtp_user": "sim.montali@gmail.com",
    "smtp_password": "realpassword!",
    "mail_sender": "sim.montali@gmail.com",
    "mail_sender_name": "Simone M."
}
```

Everything is now set up. You don't need to worry about anything else.



<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request



<!-- LICENSE -->
## License

Distributed under the GPL License. See `LICENSE` for more information.



<!-- CONTACT -->
## Contact

[Simone Montali](https://monta.li) - [@Caffeina](https://caffeina.com)

Project Link: [https://github.com/simmontali/postino](https://github.com/simmontali/postino)

[screenshot]: README_res/screenshot.gif "Screenshot"