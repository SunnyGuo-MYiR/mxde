### 5.2  Add runtime library on AM335X and AM437X Series Development Boards

MEasy Web HMI back-end server is based on python tornado and D-bus, most of the runtime libraries are built by `Buildroot` except for `girepository-1.0` and `gobject-introspection`, which are stored at `myir-buildroot/board/myir/common/HMI/usr/lib`.

The main configuration of Buildroot for MEasy Web HMI is shown as below(Including the QT5 for local HMI): 


```
BR2_PACKAGE_DBUS=y
BR2_PACKAGE_DBUS_CPP=y
BR2_PACKAGE_DBUS_GLIB=y
BR2_PACKAGE_DBUS_PYTHON=y
BR2_PACKAGE_DBUS_TRIGGERD=y
# For Web HMI
BR2_PACKAGE_PYTHON=y
BR2_PACKAGE_PYTHON_SSL=y
BR2_PACKAGE_PYTHON_PYCONNMAN=y
BR2_PACKAGE_PYTHON_SETUPTOOLS=y
BR2_PACKAGE_PYTHON_SIMPLEJSON=y
BR2_PACKAGE_PYTHON_TORNADO=y
# For Local HMI
BR2_PACKAGE_QT5=y
BR2_PACKAGE_QT5BASE=y
BR2_PACKAGE_QT5BASE_LICENSE_APPROVED=y
BR2_PACKAGE_QT5BASE_XML=y
BR2_PACKAGE_QT5BASE_GUI=y
BR2_PACKAGE_QT5BASE_WIDGETS=y
BR2_PACKAGE_QT5BASE_OPENGL=y
BR2_PACKAGE_QT5BASE_OPENGL_ES2=y
BR2_PACKAGE_QT5BASE_LINUXFB=y
# BR2_PACKAGE_QT5BASE_FONTCONFIG is not set
BR2_PACKAGE_QT5BASE_GIF=y
BR2_PACKAGE_QT5BASE_JPEG=y
BR2_PACKAGE_QT5BASE_PNG=y
BR2_PACKAGE_QT5BASE_DBUS=y
BR2_PACKAGE_QT5BASE_TSLIB=y

```