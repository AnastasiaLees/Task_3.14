[ < к содержанию](./readme.md)

## git clone

**git clone — создание копии (удаленного) репозитория**

Для начала работы с центральным репозиторием, следует создать копию оригинального проекта со всей его историей локально.

Клонирует репозиторий, используя протокол **http:**

```bash=
git clone http://user@somehost:port/~user/repository/project.git
```

Клонирует репозиторий с той же машины в директорию **myrepo:**

```bash=
git clone /home/username/project myrepo
```

Клонирует репозиторий, используя безопасный протокол **ssh:**

```bash=
git clone ssh://user@somehost:port/~user/repository
```

У **git** имеется и собственный протокол:

```bash=
git clone git://user@somehost:port/~user/repository/project.git/
```

Импортирует ***svn*** репозиторий, используя протокол **http:**

```bash=
git svn clone -s http://repo/location
```

где -s – понимать стандартные папки SVN (trunk, branches, tags)