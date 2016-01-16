# ansible-archive role

## Usage
```yaml
---

#archive_name             : "myapp.tar.gz"
#archive_src              : "/src/app"
archive_dest             : "/tmp"

archive_compress         : "gzip" # "auto,bzip2 gzip, none"
archive_exclude_pattern  : False
archive_extra_options    : ""
archive_default_options  : "--create --file "

#
archive_exclude_option   : "{{ '--exclude ' + archive_exclude_pattern if archive_exclude_pattern else '' }}"
archive_compress_option  : 
                auto     : "--auto-compress"
                bzip2    : "--bzip2"
                gzip     : "--gzip"
                none     : ""
```
