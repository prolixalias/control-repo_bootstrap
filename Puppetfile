forge 'http://forge.puppetlabs.com'

def default_branch(default)
  begin
    match = /(.+)_(cdpe|cdpe_ia)_\d+$/.match(@librarian.environment.name)
    match ? match[1]:default
  rescue
    default
  end
end

# Forge modules

mod 'abuxton-pdk', '0.2.0'
mod 'puppetlabs-apt', '6.3.0'
mod 'puppetlabs-bolt_shim', '0.3.0'
mod 'puppetlabs-concat', '5.3.0'
mod 'puppetlabs-docker', '3.5.0'
mod 'puppetlabs-exec', '0.3.0'
mod 'puppetlabs-firewall', '1.15.1'
mod 'puppetlabs-git', '0.5.0'
mod 'puppetlabs-reboot', '2.1.2'
mod 'puppetlabs-stdlib', '5.2.0'
mod 'puppetlabs-translate', '1.2.0'
mod 'puppetlabs-vcsrepo', '2.4.0'

# Component modules

mod 'rgbank',
    git:            'https://github.com/puppetlabs-seteam/puppetlabs-rgbank.git',
    branch:         :control_branch,
    default_branch: default_branch('master')
