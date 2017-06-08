#increase login timeout
https://stackoverflow.com/questions/26407541/increase-the-jenkins-login-timeout

import org.kohsuke.stapler.Stapler;
Stapler.getCurrentRequest().getSession().getMaxInactiveInterval() / 60

import org.kohsuke.stapler.Stapler;
Stapler.getCurrentRequest().getSession().setMaxInactiveInterval(18000)
