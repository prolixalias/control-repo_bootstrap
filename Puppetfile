forge 'http://forge.puppetlabs.com'

def default_branch(default)
  begin
    match = /(.+)_(cdpe|cdpe_ia)_\d+$/.match(@librarian.environment.name)
    match ? match[1]:default
  rescue
    default
  end
end

# Modules from the Puppet Forge
# Versions should be updated to be the latest at the time you start
mod 'puppetlabs-apt', '6.3.0'
mod 'puppetlabs-aws', '2.1.0'
mod 'puppetlabs-azure', '1.3.1'
mod 'puppetlabs-bolt_shim', '0.3.0'
mod 'puppetlabs-concat', '5.3.0'
mod 'puppetlabs-docker', '3.5.0'
mod 'puppetlabs-exec', '0.3.0'
mod 'puppetlabs-firewall', '1.15.1'
mod 'puppetlabs-git', '0.5.0'
mod 'puppetlabs-haproxy', '3.0.1'
mod 'puppetlabs-hocon', '1.0.1'
mod 'puppetlabs-host_core', '1.0.2'
mod 'puppetlabs-ntp', '7.4.0'
mod 'puppetlabs-puppetserver_gem', '1.1.1'
mod 'puppetlabs-reboot', '2.1.2'
mod 'puppetlabs-selinux_core', '1.0.2'
mod 'puppetlabs-sshkeys_core', '1.0.2'
mod 'puppetlabs-stdlib', '5.2.0'
mod 'puppetlabs-translate', '1.2.0'
mod 'puppetlabs-vcsrepo', '2.4.0'
mod 'puppetlabs-yumrepo_core', '1.0.3'

# Forge Community Modules
# mod 'puppet-splunk', '7.3.0'    # Can't use as 7.3.0 is broken
mod 'WhatsARanjit-diskspace', '0.2.0'
mod 'WhatsARanjit-node_manager', '0.7.1'
mod 'abuxton-pdk', '0.2.0'
mod 'puppet-selinux', '1.6.1'
mod 'puppet-wget', '2.0.1'
mod 'reidmv-unzip', '0.1.2'
mod 'thias-sysctl', '1.0.6'
mod 'tkishel-system_gem', '1.1.1'
mod 'trlinkin-domain_membership', '1.1.2'
mod 'tse-time', '1.0.1'
mod 'tse-winntp', '1.0.1'
mod 'yelp-uchiwa', '2.1.0'

# replaces mod 'puppet-splunk', '7.3.0' until there is a newer release
mod 'splunk',
    git: 'https://github.com/voxpupuli/puppet-splunk.git',
    ref: 'e9500e74f8d1d0f32dd0e68f8cba1662256c39be'

mod 'tse-tse_facts',
    git: 'https://github.com/puppetlabs/tse-module-tse_facts.git',
    ref: '638abef'

mod 'rgbank',
    git:            'https://github.com/puppetlabs-seteam/puppetlabs-rgbank.git',
    branch:         :control_branch,
    default_branch: default_branch('master')

mod 'netstat',
    git: 'https://github.com/ipcrm/ipcrm-netstat.git',
    ref: '64bcee0'
