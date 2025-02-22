---
title: Visualizar paquetes
intro: Puedes ver los detalles de los paquetes que se publican en un repositorio y filtrar los resultados por organización o usuario.
product: '{% data reusables.gated-features.packages %}'
redirect_from:
  - /articles/viewing-a-repositorys-packages
  - /github/managing-packages-with-github-packages/publishing-and-managing-packages/viewing-a-repositorys-packages
  - /github/managing-packages-with-github-packages/viewing-packages
  - /packages/publishing-and-managing-packages/viewing-packages
  - /packages/manage-packages/viewing-packages
permissions: You must have at least read permissions to view a package.
versions:
  fpt: '*'
  ghes: '*'
  ghae: '*'
  ghec: '*'
ms.openlocfilehash: 49771647b9c176d50dffeab150f4597598cb6109
ms.sourcegitcommit: dc42bb4a4826b414751ffa9eed38962c3e3fea8e
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/13/2022
ms.locfileid: '145140509'
---
{% data reusables.package_registry.packages-ghes-release-stage %} {% data reusables.package_registry.packages-ghae-release-stage %}

## <a name="about-package-views"></a>Ver paquetes de un repositorio

Tu capacidad de ver un paquete depende de varios factores. Predeterminadamente, puedes ver todos los paquetes que hayas publicado. 

Los paquetes con alcance de repositorio heredan sus permisos y visibilidad desde el repositorio al que pertenece el paquete. Los siguientes registros utilizan este tipo de permisos:{% ifversion not fpt or ghec %}
- Registro de Docker (`docker.pkg.github.com`){% endif %}
- Registro de npm
- Registro de RubyGems
- Registro de Apache maven
- Registro de NuGet

{% ifversion fpt or ghec %} El registro de contenedor ofrece la opción de contar con permisos granulares y configuraciones de visibilidad que se pueden personalizar para cada paquete que pertenezca a un usuario personal o a una cuenta de organización. Puedes elegir utilizar permisos granulares o conectar el paquete a un repositorio y heredar sus permisos. Para obtener más información, consulte "[Conexión de un repositorio a un paquete](/packages/learn-github-packages/connecting-a-repository-to-a-package)".
{% endif %}

Para obtener más información, consulte "[Acerca de los permisos para paquetes de GitHub](/packages/learn-github-packages/about-permissions-for-github-packages){% ifversion fpt or ghec %}" y "[Configuración del control de acceso y visibilidad de un paquete](/packages/learn-github-packages/configuring-a-packages-access-control-and-visibility){% endif %}".

{% data reusables.package_registry.package-page-info %}

## <a name="viewing-a-repositorys-packages"></a>Visualizar los paquetes de un repositorio

Puedes encontrar y ver un paquete que se ubique en un repositorio particular.

{% data reusables.repositories.navigate-to-repo %} {% data reusables.package_registry.packages-from-code-tab %} {% data reusables.package_registry.navigate-to-packages %}

## <a name="viewing-an-organizations-packages"></a>Visualizar los paquetes de una organización

Puedes ver y encontrar un paquete que se ubique en los repositorios de una organización a la cual pertenezcas.

{% data reusables.profile.access_org %} {% data reusables.user-settings.access_org %}
3. En el nombre de la organización, haga clic en {% octicon "package" aria-label="The package icon" %} **Packages**.
{% data reusables.package_registry.navigate-to-packages %}

## <a name="viewing-your-packages"></a>Visualizar tus paquetes

Puedes encontrar y ver cualquier paquete que hayas publicado en cualquier organización y repositorio. 

{% data reusables.profile.access_profile %}
2. En la parte superior de la página del perfil, en el panel de navegación principal, haga clic en **Packages**.
  ![Pestaña Project](/assets/images/help/package-registry/user-packages-tab.png) {% data reusables.package_registry.navigate-to-packages %}

## <a name="further-reading"></a>Información adicional

- "[Búsqueda de paquetes](/search-github/searching-on-github/searching-for-packages)"
