# Vcredit-Gradle-Plugin-Repo
### 1. Gradle集成

`project`的`build.grade`中添加`maven`地址和`classpath`

    buildscript {
    repositories {
        jcenter()
        maven {
            url "https://raw.githubusercontent.com/Amarterlus/Vcredit-Gradle-Plugin-Repo/master"
        }
    }
    dependencies {
        ...
        classpath 'com.codelessda:codelessda-gradle-plugin:0.0.4'
        ...
    }
}

`app`的`build.grade`中添加
	
	// 引用远程maven仓库的插件
    apply plugin: 'com.vcredit'