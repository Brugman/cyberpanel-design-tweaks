# CyberPanel Design Tweaks

> Tweak the look of CyberPanel to your liking by adding CSS snippets to your custom CSS on the Design page.

## Tweaks

### Remove page loader

```css
/* Remove page loader */
#loading{height:0%;overflow:hidden}
```

### Remove new badges

```css
/* Remove new badges */
#sidebar-menu li span.bs-label.badge-yellow{display:none}
```

### Remove menu icon wiggle

```css
/* Remove menu icon wiggle */
#page-sidebar li a:hover .glyph-icon{animation-name:none}
```

### Replace Raleway font with Open Sans

```css
/* Replace Raleway font with Open Sans */
#page-title>h2,#page-title>p,h1,h2,h3,h4,h5,h6{font-family:inherit}
```

### Apply flexbox to panels

```css
/* Apply flexbox to panels */
.col-md-3.panel-body,.col-md-6.panel-body{display:flex;justify-content:flex-start;align-items:center;padding:15px 0}
```

### Dark mode alerts

```css
/* Dark mode alerts */
.alert-success,.alert-success a,.parsley-success{background-color:rgba(46,204,113,.1);border-left:4px solid #2ecc71;color:#fff}.alert-danger,.alert-danger a,.danger,.parsley-error{background-color:rgba(231,76,60,.1);border-left:4px solid #e74c3c;color:#fff}
```

### Style server IP like normal

```css
/* Style server IP like normal */
#sidebar-menu-item-server-ip-address span{font-weight:400!important;color:inherit!important}
```

### Hide menu items

Remove menu items you want to keep from this list.

```css
/* Hide menu items */
#sidebar-menu-item-server-ip-address,
#sidebar-menu-item-dashboard,
#sidebar-menu-item-version-management,
#sidebar-menu-item-design,
#sidebar-menu-item-connect,
#sidebar-menu-item-community,
#sidebar-menu-item-users,
#sidebar-menu-item-wordpress,
#sidebar-menu-item-websites,
#sidebar-menu-item-packages,
#sidebar-menu-item-databases,
#sidebar-menu-item-email,
#sidebar-menu-item-ftp,
#sidebar-menu-item-backup,
#sidebar-menu-item-incremental-backup,
#sidebar-menu-item-ssl,
#sidebar-menu-item-root-file-manager,
#sidebar-menu-item-cloudlinux,
#sidebar-menu-item-containerization,
#sidebar-menu-item-docker,
#sidebar-menu-item-tuning,
#sidebar-menu-item-server-status,
#sidebar-menu-item-php,
#sidebar-menu-item-logs,
#sidebar-menu-item-security,
#sidebar-menu-item-mail-settings,
#sidebar-menu-item-manage-services,
#sidebar-menu-item-plugins {
    display: none !important;
}
```

## Contributing

Found a bug? Anything you would like to ask, add or change? Please open an issue so we can talk about it.

Pull requests are welcome. Please try to match the current code formatting.

## Development

### Requirements

- [NodeJS](https://nodejs.org/en/)

### Installation

1. `pnpm i`

### Build CSS

Command | Action
:--- |:---
`pnpm gulp` | Build once
`pnpm gulp watch` | Build continuously

## Author

[Tim Brugman](https://github.com/Brugman)
