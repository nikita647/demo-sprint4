// Folder Definitions
folder('Job-DSL') {
    displayName('Job-DSL')
}

folder('Job-DSL/Env') {
    displayName('Env')
}

folder('Job-DSL/Env/Dev') {
    displayName('Dev')
}

folder('Job-DSL/Env/Dev/CI') {
    displayName('CI')
}

folder('Job-DSL/Env/Dev/CI/Ansible') {
    displayName('Ansible')
}

folder('Job-DSL/Env/Dev/CI/Ansible/Role') {
    displayName('Role')
}

folder('Job-DSL/Env/Dev/CI/Ansible/Role/Redis') {
    displayName('Redis')
}

folder('Job-DSL/Env/Dev/CI/Ansible/Role/PostgreSQL') {
    displayName('PostgreSQL')
}

folder('Job-DSL/Env/Dev/CI/Ansible/Role/ScyllaDB') {
    displayName('ScyllaDB')
}


folder('Job-DSL/Env/Dev/CD') {
    displayName('CD')
}

folder('Job-DSL/Env/Dev/CD/Delivery') {
    displayName('Delivery')
}

folder('Job-DSL/Env/Dev/CD/Delivery/Ansible') {
    displayName('Ansible')
}

folder('Job-DSL/Env/Dev/CD/Delivery/Ansible/Role') {
    displayName('Role')
}

folder('Job-DSL/Env/Dev/CD/Delivery/Ansible/Role/Redis') {
    displayName('Redis')
}

folder('Job-DSL/Env/Dev/CD/Delivery/Ansible/Role/PostgreSQL') {
    displayName('PostgreSQL')
}
folder('Job-DSL/Env/Dev/CD/Delivery/Ansible/Role/ScyllaDB') {
    displayName('ScyllaDB')
}


folder('Job-DSL/Env/Dev/CD/Deployment') {
    displayName('Deployment')
}

folder('Job-DSL/Env/Dev/CD/Deployment/Ansible') {
    displayName('Ansible')
}

folder('Job-DSL/Env/Dev/CD/Deployment/Ansible/Role') {
    displayName('Role')
}

folder('Job-DSL/Env/Dev/CD/Deployment/Ansible/Role/Redis') {
    displayName('Redis')
}

folder('Job-DSL/Env/Dev/CD/Deployment/Ansible/Role/PostgreSQL') {
    displayName('PostgreSQL')
}

folder('Job-DSL/Env/Dev/CD/Deployment/Ansible/Role/ScyllaDB') {
    displayName('ScyllaDB')
}

folder('Job-DSL/Env/Dev/Infra') {
    displayName('Infra')
}

folder('Job-DSL/Env/Dev/Infra/Application') {
    displayName('Application')
}

folder('Job-DSL/Env/Dev/Infra/Application/Frontend') {
    displayName('Frontend')
}

folder('Job-DSL/Env/Dev/Infra/Application/Salary') {
    displayName('Salary')
}

folder('Job-DSL/Env/Dev/Infra/Application/Employee') {
    displayName('Employee')
}

folder('Job-DSL/Env/Dev/Infra/Application/Attendance') {
    displayName('Attendance')
}
folder('Job-DSL/Env/Dev/Infra/Application/Network Skeleton') {
    displayName('Frontend')
}

folder('Job-DSL/Env/Dev/Infra/Database') {
    displayName('Database')
}

folder('Job-DSL/Env/Dev/Infra/Database/Redis') {
    displayName('Redis')
}

folder('Job-DSL/Env/Dev/Infra/Database/PostgreSQL') {
    displayName('PostgreSQL')
}

folder('Job-DSL/Env/Dev/Infra/Database/ScyllaDB') {
    displayName('ScyllaDB')
}


job('Job-DSL/Env/Dev/CD/Delivery/Ansible/Role/Redis/Job-DSL') {
    displayName('Job-DSL')
    description('Job to deploy Redis from GitHub repository')

    scm {
        git {
            remote {
                url('https://github.com/snaatak-Zero-Downtime-Crew/job-dsl.git')
                credentials('git-cred')
            }
            branch('Sharvari-SCRUM-323')
        }
    }

    steps {
        // Use setScriptText for Groovy script
        dsl {
            external('CD/Ansible/Role/Redis/Ansible_CD.groovy')
            lookupStrategy('SEED_JOB')
        }
    }
 
}

job('Job-DSL/Env/Dev/CD/Delivery/Ansible/Role/PostgreSQL/Job-DSL') {
    displayName('Job-DSL')
    description('Job to deploy PostgreSQL from GitHub repository')

    scm {
        git {
            remote {
                url('https://github.com/snaatak-Zero-Downtime-Crew/job-dsl.git')
                credentials('git-cred')
            }
            branch('Anuj-SCRUM-318')
        }
    }

    steps {
        // Use setScriptText for Groovy script
        dsl {
            external('CD/Ansible/Role/Postgres/Ansible_CD.groovy')
            lookupStrategy('SEED_JOB')
        }
    }
 
}

job('Job-DSL/Env/Dev/CD/Delivery/Ansible/Role/ScyllaDB/Job-DSL') {
    displayName('Job-DSL')
    description('Job to deploy ScyllaDB from GitHub repository')

    scm {
        git {
            remote {
                url('https://github.com/snaatak-Zero-Downtime-Crew/job-dsl.git')
                credentials('git-cred')
            }
            branch('Pravesh-SCRUM-313')
        }
    }

    steps {
        // Use setScriptText for Groovy script
        dsl {
            external('CD/ScyllaDB/scyllaDB.groovy')
            lookupStrategy('SEED_JOB')
        }
    }
 
}

job('Job-DSL/Env/Dev/Infra/Database/PostgreSQL/Job-DSL') {
    displayName('Job-DSL')
    description('Job PostgreSQL Infra from GitHub repository')

    scm {
        git {
            remote {
                url('https://github.com/snaatak-Zero-Downtime-Crew/job-dsl.git')
                credentials('git-cred')
            }
            branch('Shashi-SCRUM-310')
        }
    }

    steps {
        // Use setScriptText for Groovy script
        dsl {
            external('Infra/Database/PostgreSQL/infra.groovy')
            lookupStrategy('SEED_JOB')
        }
    }
 
}


job('Job-DSL/Env/Dev/Infra/Database/ScyllaDB/Job-DSL') {
    displayName('Job-DSL')
    description('Job ScyllaDB Infra from GitHub repository')

    scm {
        git {
            remote {
                url('https://github.com/snaatak-Zero-Downtime-Crew/job-dsl.git')
                credentials('git-cred')
            }
            branch('Shubhanshi-SCRUM-307')
        }
    }

    steps {
        // Use setScriptText for Groovy script
        dsl {
            external('Infra/Database/Scylla/DSLScript.groovy')
            lookupStrategy('SEED_JOB')
        }
    }
 
}


job('Job-DSL/Env/Dev/Infra/Database/Redis/Job-DSL') {
    displayName('Job-DSL')
    description('Job Redis Infra from GitHub repository')

    scm {
        git {
            remote {
                url('https://github.com/snaatak-Zero-Downtime-Crew/job-dsl.git')
                credentials('git-cred')
            }
            branch('Sharvari-SCRUM-304')
        }
    }

    steps {
        // Use setScriptText for Groovy script
        dsl {
            external('Infra/Database/Redis/infra.groovy')
            lookupStrategy('SEED_JOB')
        }
    }
 
}


job('Job-DSL/Env/Dev/Infra/Application/Employee/Job-DSL') {
    displayName('Job-DSL')
    description('Job Employee Infra from GitHub repository')

    scm {
        git {
            remote {
                url('https://github.com/snaatak-Zero-Downtime-Crew/job-dsl.git')
                credentials('git-cred')
            }
            branch('Prashant-SCRUM-301')
        }
    }

    steps {
        // Use setScriptText for Groovy script
        dsl {
            external('Static/Dev Infra/Applications/Employee/DSLScript.groovy')
            lookupStrategy('SEED_JOB')
        }
    }
 
}


job('Job-DSL/Env/Dev/Infra/Application/Salary/Job-DSL') {
    displayName('Job-DSL')
    description('Job Salary Infra from GitHub repository')

    scm {
        git {
            remote {
                url('https://github.com/snaatak-Zero-Downtime-Crew/job-dsl.git')
                credentials('git-cred')
            }
            branch('Aman-SCRUM-294')
        }
    }

    steps {
        // Use setScriptText for Groovy script
        dsl {
            external('Static/Dev Infra/Applications/Salary/DSLScript.groovy')
            lookupStrategy('SEED_JOB')
        }
    }
 
}


job('Job-DSL/Env/Dev/Infra/Application/Attendance/Job-DSL') {
    displayName('Job-DSL')
    description('Job Attendance Infra from GitHub repository')

    scm {
        git {
            remote {
                url('https://github.com/snaatak-Zero-Downtime-Crew/job-dsl.git')
                credentials('git-cred')
            }
            branch('Shubhanshi-SCRUM-287')
        }
    }

    steps {
        // Use setScriptText for Groovy script
        dsl {
            external('Static/Dev Infra/Applications/Attendance/DSLScript.groovy')
            lookupStrategy('SEED_JOB')
        }
    }
 
}

job('Job-DSL/Env/Dev/Infra/Application/Frontend/Job-DSL') {
    displayName('Job-DSL')
    description('Job Frontend Infra from GitHub repository')

    scm {
        git {
            remote {
                url('https://github.com/snaatak-Zero-Downtime-Crew/job-dsl.git')
                credentials('git-cred')
            }
            branch('Rohit-SCRUM-280')
        }
    }

    steps {
        // Use setScriptText for Groovy script
        dsl {
            external('Static/Dev Infra/Applications/Frontend/DSLScript.groovy')
            lookupStrategy('SEED_JOB')
        }
    }
 
}


job('Job-DSL/Env/Dev/Infra/Application/Network Skeleton/Job-DSL') {
    displayName('Job-DSL')
    description('Job Frontend Infra from GitHub repository')

    scm {
        git {
            remote {
                url('https://github.com/snaatak-Zero-Downtime-Crew/job-dsl.git')
                credentials('git-cred')
            }
            branch('main')
        }
    }

    steps {
        // Use setScriptText for Groovy script
        dsl {
            external('Static/Dev Infra/Network Skeleton/DSLscript.groovy')
            lookupStrategy('SEED_JOB')
        }
    }
 
}

job('Job-DSL/Env/Dev/CD/Deployment/Ansible/Role/Redis/Job-DSL') {
    displayName('Job-DSL')
    description('Job For Redis configuration from GitHub repository')

    scm {
        git {
            remote {
                url('https://github.com/snaatak-Zero-Downtime-Crew/job-dsl.git')
                credentials('git-cred')
            }
            branch('Nikita-SCRUM-325')
        }
    }

    steps {
        // Use setScriptText for Groovy script
        dsl {
            external('CD/Configuration/Redis/DSLScript.groovy')
            lookupStrategy('SEED_JOB')
        }
    }
 
}



job('Job-DSL/Env/Dev/CD/Deployment/Ansible/Role/PostgeSQL/Job-DSL') {
    displayName('Job-DSL')
    description('Job For PostgeSQL configuration from GitHub repository')

    scm {
        git {
            remote {
                url('https://github.com/snaatak-Zero-Downtime-Crew/job-dsl.git')
                credentials('git-cred')
            }
            branch('Aayush-SCRUM-320')
        }
    }

    steps {
        // Use setScriptText for Groovy script
        dsl {
            external('CD/Postgresql/Configuration/DSLScript.groovy')
            lookupStrategy('SEED_JOB')
        }
    }
 
}


job('Job-DSL/Env/Dev/CD/Deployment/Ansible/Role/ScyllaDB/Job-DSL') {
    displayName('Job-DSL')
    description('Job For ScyllaDB configuration from GitHub repository')

    scm {
        git {
            remote {
                url('https://github.com/snaatak-Zero-Downtime-Crew/job-dsl.git')
                credentials('git-cred')
            }
            branch('Pooja-SCRUM-315')
        }
    }

    steps {
        // Use setScriptText for Groovy script
        dsl {
            external('CD/Scylladb/Configuration/DSLScript.groovy')
            lookupStrategy('SEED_JOB')
        }
    }
 
}


job('Job-DSL/Env/Dev/CI/Ansible/Role/Redis/Job-DSL') {
    displayName('Job-DSL')
    description('Job For Redis CI from GitHub repository')

    scm {
        git {
            remote {
                url('https://github.com/snaatak-Zero-Downtime-Crew/job-dsl.git')
                credentials('git-cred')
            }
            branch('Aman-SCRUM-322')
        }
    }

    steps {
        // Use setScriptText for Groovy script
        dsl {
            external('CI/Redis/DSLScript.groovy')
            lookupStrategy('SEED_JOB')
        }
    }
 
}


job('Job-DSL/Env/Dev/CI/Ansible/Role/PostgreSQL/Job-DSL') {
    displayName('Job-DSL')
    description('Job For PostgreSQL CI from GitHub repository')

    scm {
        git {
            remote {
                url('https://github.com/snaatak-Zero-Downtime-Crew/job-dsl.git')
                credentials('git-cred')
            }
            branch('Mohit-SCRUM-317')
        }
    }

    steps {
        // Use setScriptText for Groovy script
        dsl {
            external('CI/Postgres/DSLScript.groovy')
            lookupStrategy('SEED_JOB')
        }
    }
 
}


job('Job-DSL/Env/Dev/CI/Ansible/Role/ScyllaDB/Job-DSL') {
    displayName('Job-DSL')
    description('Job For ScyllaDB CI from GitHub repository')

    scm {
        git {
            remote {
                url('https://github.com/snaatak-Zero-Downtime-Crew/job-dsl.git')
                credentials('git-cred')
            }
            branch('Ramratan-SCRUM-312')
        }
    }

    steps {
        // Use setScriptText for Groovy script
        dsl {
            external('CI/Scylla_DB/Job_DSL.groovy')
            lookupStrategy('SEED_JOB')
        }
    }
 
}
