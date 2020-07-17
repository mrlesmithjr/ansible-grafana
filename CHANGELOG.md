commit db8558314148a03f4b7e48d58a64d4b0825373f6
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Fri Jul 17 01:43:25 2020 -0400

    Updated Python requirements

commit 51100b9062825f781cec53d0836b51eb6efaff7f
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Fri Jul 17 01:43:14 2020 -0400

    Updated CI tests to latest

commit 35cd057eab61747622b3b2775a1755cfc6efdbfe
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Sat Jul 11 18:18:27 2020 -0400

    Added ability to load dashboards
    
    This adds the ability to load dashboards during provisioning. The
    datasources will typically need to be changed.

commit a8231dea9425c97db3694326f48ed8b27c20bcb4
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Wed Jul 8 09:08:51 2020 -0400

    Fixed issue with pre-loading Datasources
    
    When attempting to manage datasources and the password was changed,
    failures started occuring.

commit 6214bc3e1765b2bdf32f959edaf0f782c7debd09
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Sun Jul 5 11:23:21 2020 -0400

    Added ability to serve from sub_path
    
    https://grafana.com/tutorials/run-grafana-behind-a-proxy/#1

commit 1ea9cf4524154bdb85aaa1c2772a2e8fce1f69da
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Tue Apr 7 11:42:20 2020 -0400

    Disabled Fedora testing for now

commit 63f5232318e1050a05d2e1e31848ba83f699c407
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Tue Apr 7 11:20:24 2020 -0400

    Fixed CentOS repo and package install

commit fdf5a2798e13e6139007a4d577020f3c2d2944f9
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Tue Apr 7 10:16:09 2020 -0400

    Refactored tasks, etc.

commit 312c001089dd0ee6c7951599edcc26d10e276fee
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Tue Apr 7 09:42:39 2020 -0400

    Removed old vSphere support

commit acca3f99f54de29311b702ec24a9042b1fff02c6
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Tue Apr 7 09:35:46 2020 -0400

    Added: New files, etc. from cookiecutter template

commit 507556ef013a5cea0cee7cb13b6bd556f4e3bf4e
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Tue Apr 7 09:35:22 2020 -0400

    Updated files, etc. after new structure
    
    This aligns to cookiecutter template

commit b6f063fec68833a914427d6857f1f7103292ea1b
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Tue Apr 7 09:32:54 2020 -0400

    Added: New files, etc. from cookiecutter template

commit f885f9f4d205bbbccf36ad1ad4b4f89c97fafdf9
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Tue Apr 7 09:32:24 2020 -0400

    Deleted old tests, etc. not needed
    
    These files are no longer required for new format

commit ba60cec10708c511f1daccd5974b8203cb5359d7
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Fri Dec 28 23:15:49 2018 -0500

    Added missing apt-transport-https pre-req

commit 7d5b6c4dd1b76db482216e57e268d9c41320fada
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Fri Dec 28 23:11:02 2018 -0500

    Changed order of pre-reqs to ensure gpg is available

commit 3044a3f3541cebea23b16ad3d6fcc920b50e2be7
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Fri Dec 28 23:06:47 2018 -0500

    Added missing pre-req for gpg

commit 953f7949bc5884cc8e4eda0b6ed2092580371117
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Fri Dec 28 23:01:58 2018 -0500

    Refactored code
    
    Cleaned up code based on Ansible lint and YAML lint
    Implemented updated Travis CI testing

commit 93b13383bf8bc467fe17c6388c18012df4e8d0e3
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Tue Sep 4 20:13:39 2018 -0400

    Cleaned up repo info

commit 9976b8b43b19b0b59ce3e7d417ef74a3f991a22d
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Tue Sep 4 20:13:28 2018 -0400

    Added ability to manage datasources and change method for managing plugins

commit 257c6c17ae26c5e2cc8290f9974af728be4ef8ba
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Mon Feb 19 21:55:25 2018 -0500

    Updated repo info

commit 30cab92f5fb4b09a037b07363ff4a22a784c6b26
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Mon Feb 19 21:55:17 2018 -0500

    Updated Ansible Galaxy meta info

commit 56b55033b60b8f1e017bc097ae484e087f1362fb
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Mon Feb 19 21:54:59 2018 -0500

    Cleaned up formatting

commit 3fdf6a8d261837555782844995c3c55e81ed24ed
Author: KrE80r <KrE80r@users.noreply.github.com>
Date:   Sat Dec 9 16:37:36 2017 +0400

    Update provision.sh
    
    Support for  newer versions of Ansible/setuptools

commit 7b59cf4c4ea5a37ef5f818aee0962b5febdf4383
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Tue May 2 13:25:30 2017 -0400

    Changed formatting of code/logic for cleanliness
    
    Signed-off-by: Larry Smith Jr <mrlesmithjr@gmail.com>

commit 64e95957ea8caa073de3beac671ebda8c5e2f0af
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Sun Dec 18 08:57:20 2016 -0500

    Fixed merge conflict
    
    Signed-off-by: Larry Smith Jr <mrlesmithjr@gmail.com>

commit 6b610dd15a823cf2db3e3bd1119084f9be8343f8
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Sun Dec 18 08:53:13 2016 -0500

    Cleaned up variable naming for a cleaner namespace
    
    Signed-off-by: Larry Smith Jr <mrlesmithjr@gmail.com>

commit 59e5fe0f093b1eb6b7b59068cbac57c8f8c9f8c9
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Sun Dec 18 08:52:49 2016 -0500

    Added example dashboards
    
    Signed-off-by: Larry Smith Jr <mrlesmithjr@gmail.com>

commit fc585a39cbe0318fc54387fa96ae48d4795aa59c
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Fri Oct 21 01:33:27 2016 -0400

    Changed default for enable_grafana_plugins to false
    
    Signed-off-by: Larry Smith Jr <mrlesmithjr@gmail.com>

commit 51a3c6b0f8b79f266f71cafd3deca06e28ba9e61
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Thu Oct 20 20:39:12 2016 -0400

    Added Travis testing
    
    Signed-off-by: Larry Smith Jr <mrlesmithjr@gmail.com>

commit de0ae12d8bf4473e079fa3ad09b46046b60edd23
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Thu Oct 20 20:33:17 2016 -0400

    Updated repo info
    
    Signed-off-by: Larry Smith Jr <mrlesmithjr@gmail.com>

commit 0add296f760ca5b97ff3f00e3cfdc28f17e5669d
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Thu Oct 20 20:29:44 2016 -0400

    Complete rewrite
    
    Signed-off-by: Larry Smith Jr <mrlesmithjr@gmail.com>

commit 5cff7361506f7e0d46d7ec5d5bca845fe0dcb25d
Author: Larry Smith Jr <mrlesmithjr@gmail.coml>
Date:   Sun Jan 24 22:53:18 2016 -0500

    Added login info and made script executable
    
    Signed-off-by: Larry Smith Jr <mrlesmithjr@gmail.coml>

commit da471e18f15fcaffc9506083c0520ad6e8cf99ef
Author: Larry Smith Jr <mrlesmithjr@gmail.coml>
Date:   Sun Jan 24 22:44:53 2016 -0500

    Changed naming of file
    
    Signed-off-by: Larry Smith Jr <mrlesmithjr@gmail.coml>

commit b7fab94f2c6f300d9380498d7f7e16511d71c1fd
Author: Larry Smith Jr <mrlesmithjr@gmail.coml>
Date:   Sun Jan 24 22:38:26 2016 -0500

    Added missing folder
    
    Signed-off-by: Larry Smith Jr <mrlesmithjr@gmail.coml>

commit 1c307f30e6ab104d4cf27ddc792004bac6d2549f
Author: Larry Smith Jr <mrlesmithjr@gmail.coml>
Date:   Sun Jan 24 22:29:56 2016 -0500

    Added missing vsphere-sdk
    
    Signed-off-by: Larry Smith Jr <mrlesmithjr@gmail.coml>

commit c6cbb14d63252b5d17bb3fec384047e43870a8ec
Author: Larry Smith Jr <mrlesmithjr@gmail.coml>
Date:   Sun Jan 24 21:52:36 2016 -0500

    Added Vagrant build info
    
    Signed-off-by: Larry Smith Jr <mrlesmithjr@gmail.coml>

commit 21b2022c7e811ed33cdbd1b8492e4dbf84e46efc
Author: Larry Smith Jr <mrlesmithjr@gmail.coml>
Date:   Sun Jan 24 21:52:18 2016 -0500

    Cleaned up formatting of tasks
    
    Signed-off-by: Larry Smith Jr <mrlesmithjr@gmail.coml>

commit 8c069598642a8f503e48f3522e2ae5ec52983af6
Author: Larry Smith Jr <mrlesmithjr@gmail.com>
Date:   Mon Oct 26 21:20:15 2015 -0400

    removed dependencies

commit 89f998e350cb22e61b0de913f2a542fabaa97cab
Author: Larry Smith Jr <larry.e.smith.jr@gmail.com>
Date:   Wed Jul 29 16:47:04 2015 -0400

    updating tasks

commit 9c1bdb426ada0c9e7d1d4dcc4df82bbbe33bafcb
Author: Larry Smith Jr <larry.e.smith.jr@gmail.com>
Date:   Wed Jul 29 16:16:32 2015 -0400

    first commit
